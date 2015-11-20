# roll-dice-animation
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace zar_animasyonu
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
           int dice1, dice2;
            Random rnd = new Random();
            dice1 = rnd.Next(1, 7);
            dice2 = rnd.Next(1, 7);
            if (dice1 == 1)
            {
                //pictureBox1.Load(@"Properties.Resources.resx.1.jpg");
                pictureBox1.Image = Properties.Resources._1;
            }
            if (dice1 == 2)
            {
               // pictureBox1.Load(@"C:\Users\Kullanıcıname\Desktop\2.jpg");
                pictureBox1.Image = Properties.Resources._2;
            }
            if (dice1 == 3)
            {
               // pictureBox1.Load(@"C:\Users\Kullanıcıname\Desktop\3.jpg");
                pictureBox1.Image = Properties.Resources._3;
            }
            if (dice1 == 4)
            {
                //pictureBox1.Load(@"C:\Users\Kullanıcıname\Desktop\4.jpg");
                pictureBox1.Image = Properties.Resources._4;
            }
            if (dice1 == 5)
            {
                //pictureBox1.Load(@"C:\Users\Kullanıcıname\Desktop\5.jpg");
                pictureBox1.Image = Properties.Resources._5;
            }
            if (dice1 == 6)
            {
                //pictureBox1.Load(@"C:\Users\Kullanıcıname\Desktop\6.jpg");
                pictureBox1.Image = Properties.Resources._6;
            }
            if (dice2 == 1)
            {
                //pictureBox2.Load(@"C:\Users\Kullanıcıname\Desktop\1.jpg");
                pictureBox2.Image = Properties.Resources._1;
            }
            if (dice2 == 2)
            {
               // pictureBox2.Load(@"C:\Users\Kullanıcıname\Desktop\2.jpg");
                pictureBox2.Image = Properties.Resources._2;
            } if (dice2 == 3)
            {
                //pictureBox2.Load(@"C:\Users\Kullanıcıname\Desktop\3.jpg");
                pictureBox2.Image = Properties.Resources._3;
            } if (dice2 == 4)
            {
                //pictureBox2.Load(@"C:\Users\Kullanıcıname\Desktop\4.jpg");
                pictureBox2.Image = Properties.Resources._4;
            }
            if (dice2 == 5)
            {
                //pictureBox2.Load(@"C:\Users\Kullanıcıname\Desktop\5.jpg");
                pictureBox2.Image = Properties.Resources._5;
            }
            if (dice2 == 6)
            {
                //pictureBox2.Load(@"C:\Users\Kullanıcıname\Desktop\6.jpg");
                pictureBox2.Image = Properties.Resources._6;

            }
            
            listBox1.Items.Add(dice1 + "      -       " + dice2+"               "+"1/36");


        }

        private void pictureBox1_Click(object sender, EventArgs e)
        {

        }

        private void Form1_Load(object sender, EventArgs e)
        {
            this.Text = "Zar Simülasyonu";
            listBox1.Text = "";
        }

        private void button2_Click(object sender, EventArgs e)
        {
            listBox1.Items.Remove(listBox1.SelectedItem);
        }

        private void button2_Click_1(object sender, EventArgs e)
        {
            Close();
        }
    }
}

       

     

