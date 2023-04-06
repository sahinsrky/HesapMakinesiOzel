Uygulama eğlence amaçlı yazılmıştır.
Netframework 6 kullanıldı.
winForm uygulaması.
Sorular ve öneriler için yazın.

KODLAR
{
namespace Garip_Uygulama_Yapcam
{
    public partial class Form1 : Form
    {
        double ilkrakam;
        string islem;
        double sonrakam;
        double sonuc;
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
            {
                textBox1.Text = "1";
            }
            else
            {
                textBox1.Text = textBox1.Text + "1";
            }
        }

        private void button2_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
            {
                textBox1.Text = "2";
            }
            else
            {
                textBox1.Text = textBox1.Text + "2";
            }
        }

        private void button3_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
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
            if (textBox1.Text == "0" && textBox1.Text == null)
            {
                textBox1.Text = "4";
            }
            else
            {
                textBox1.Text = textBox1.Text + "4";
            }
        }

        private void button5_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
            {
                textBox1.Text = "5";
            }
            else
            {
                textBox1.Text = textBox1.Text + "5";
            }
        }

        private void button6_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
            {
                textBox1.Text = "6";
            }
            else
            {
                textBox1.Text = textBox1.Text + "6";
            }
        }

        private void button7_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
            {
                textBox1.Text = "7";
            }
            else
            {
                textBox1.Text = textBox1.Text + "7";
            }
        }

        private void button8_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
            {
                textBox1.Text = "8";
            }
            else
            {
                textBox1.Text = textBox1.Text + "8";
            }
        }

        private void button9_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0" && textBox1.Text == null)
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
            if (textBox1.Text == "0" && textBox1.Text == null)
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
            ilkrakam = Convert.ToDouble(textBox1.Text);

            textBox1.Text = null;

            islem = "+";
        }

        private void button12_Click(object sender, EventArgs e)
        {
            ilkrakam = Convert.ToDouble(textBox1.Text);

            textBox1.Text = null;

            islem = "-";
        }

        private void button15_Click(object sender, EventArgs e)
        {
            ilkrakam = Convert.ToDouble(textBox1.Text);

            textBox1.Text = null;

            islem = "*";
        }

        private void button13_Click(object sender, EventArgs e)
        {
            ilkrakam = Convert.ToDouble(textBox1.Text);

            textBox1.Text = null;

            islem = "/";
        }

        private void button14_Click(object sender, EventArgs e)
        {
            ilkrakam = Convert.ToDouble(textBox1.Text);

            textBox1.Text = null;

            islem = "%";
        }

        //S�PR�Z BUTON ���N �ZLEMEYE DEVAM ET :)
        private void button16_Click(object sender, EventArgs e)
        {
            timer1.Start();
            button1.Text = "83N";
            button2.Text = "5AN4";
            button3.Text = "8A5M4";
            button4.Text = "D3M3D1M";
            button5.Text = "M1 ?";
            button6.Text = "M4D3M";
            button7.Text = "0YL3";
            button8.Text = "AB0N3";
            button9.Text = "0L :)";
            button10.Text = "L1K3 4T";
            button11.Text = "3M3�3";
            button12.Text = "SAYGI :)";
            button13.Text = "Y0RUM";
            button14.Text = "DA YAP";
            button15.Text = "0Y";
            button17.Text = "Y0RULDUM";
            button18.Text = "HAD� G�R���R�Z";
            textBox1.Text = "B� KEREDE S�Z D�NLEY�N YA :D";
        }

        private void button17_Click(object sender, EventArgs e)
        {
            textBox1.Text = "";
        }

        private void button18_Click(object sender, EventArgs e)
        {
            sonrakam = Convert.ToDouble(textBox1.Text);
            if (islem == "+")
            {
                sonuc = (ilkrakam + sonrakam);
                textBox1.Text = Convert.ToString(sonuc);
                ilkrakam = sonuc;
            }

            if (islem == "-")
            {
                sonuc = (ilkrakam - sonrakam);
                textBox1.Text = Convert.ToString(sonuc);
                ilkrakam = sonuc;
            }

            if (islem == "*")
            {
                sonuc = (ilkrakam * sonrakam);
                textBox1.Text = Convert.ToString(sonuc);
                ilkrakam = sonuc;
            }

            if (islem == "/")
                if (sonrakam == 0)
                {
                    textBox1.Text = "B�L�NEMEZ.!";
                }
                else
                {
                    sonuc = (ilkrakam / sonrakam);
                    textBox1.Text = Convert.ToString(sonuc);
                    ilkrakam = sonuc;
                }

            if (islem == "%")
            {
                sonuc = (ilkrakam * sonrakam / 100);
                textBox1.Text = Convert.ToString(sonuc);
                ilkrakam = sonuc;
            }
        }

        private void textBox1_KeyDown(object sender, KeyEventArgs e)
        {
            if (e.KeyCode == Keys.Enter) //textboxda entere bas�nca i�lemi ger�ekle�tirmesi i�in.
            {
                button18.PerformClick();
            }
        }

        private void timer1_Tick(object sender, EventArgs e)
        {
            MessageBox.Show("Abone Ol L�tfen :)");
        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        {

        }
    }
}
}
