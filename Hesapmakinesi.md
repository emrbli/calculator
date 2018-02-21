//# hesap makinesi için bir textbox ve 16 adet button ekleyip kodları giriyoruz
//c# hesap makinesi
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApplication2
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }
        double sayi1, sayi2,sonuc,top=0,cik=0,carp=0,bol=0;
        private void button3_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "3";
            }
            else
            {
                textBox1.Text = textBox1.Text + "3";
            }           

        }

        private void button4_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "4";
            }
            else
            {
                textBox1.Text = textBox1.Text + "4";
            }
        }

        private void button1_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "1";
            }
            else
            {
                textBox1.Text = textBox1.Text + "1";
            }
        }

        private void button6_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "6";
            }
            else
            {
                textBox1.Text = textBox1.Text + "6";
            }
        }

        private void button8_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "8";
            }
            else
            {
                textBox1.Text = textBox1.Text + "8";
            }
        }

        private void button2_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "2";
            }
            else
            {
                textBox1.Text = textBox1.Text + "2";
            }
        }

        private void button5_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "5";
            }
            else
            {
                textBox1.Text = textBox1.Text + "5";
            }
        }

        private void button7_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "7";
            }
            else
            {
                textBox1.Text = textBox1.Text + "7";
            }
        }

        private void button9_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            {
                textBox1.Text = "9";
            }
            else
            {
                textBox1.Text = textBox1.Text + "9";
            }
        }

        private void button10_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.IndexOf('+') != -1 || textBox1.Text.IndexOf('-') != -1 || textBox1.Text.IndexOf('x') != -1 || textBox1.Text.IndexOf('/') != -1)
            { 
                 textBox1.Text = "0";
            }
            else
            {
                textBox1.Text = textBox1.Text + "0";
            }
        }

        private void button11_Click(object sender, EventArgs e)
        {
            textBox1.Clear();
        }

        private void button13_Click(object sender, EventArgs e)
        {
            top = top + 1;
            sayi1=Double.Parse(textBox1.Text);
            textBox1.Text = "+";
            
        }
        private void button14_Click(object sender, EventArgs e)
        {
            cik = cik + 1;
            sayi1 = Double.Parse(textBox1.Text);
            textBox1.Text = "-";

        }

        private void button15_Click(object sender, EventArgs e)
        {
            carp = carp + 1;
            sayi1 = Double.Parse(textBox1.Text);
            textBox1.Text = "x";

        }

        private void button16_Click(object sender, EventArgs e)
        {
            bol = bol + 1;
            sayi1 = Double.Parse(textBox1.Text);
            textBox1.Text = "/";

        }

        private void button12_Click(object sender, EventArgs e)
        {
            sayi2 = Double.Parse(textBox1.Text);
            if (top==1)
            {
                sonuc = sayi1 + sayi2; 
            }
            else if (cik==1)
            {
                sonuc = sayi1 - sayi2; 
            }
            else if (carp == 1)
            {
                sonuc = sayi1 * sayi2;
            }
            else
            {
                sonuc = sayi1 / sayi2;
            }
            
            textBox1.Text = sonuc.ToString();
        }
        
    }   
}
