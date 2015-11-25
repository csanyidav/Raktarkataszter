# Raktarkataszter
RFT órára beadandó feladat

namespace Raktarkataszter
{
    partial class Raktarkataszter
    {
        /// <summary>
        /// Required designer variable.
        /// </summary>
        private System.ComponentModel.IContainer components = null;

        /// <summary>
        /// Clean up any resources being used.
        /// </summary>
        /// <param name="disposing">true if managed resources should be disposed; otherwise, false.</param>
        protected override void Dispose(bool disposing)
        {
            if (disposing && (components != null))
            {
                components.Dispose();
            }
            base.Dispose(disposing);
        }

        #region Windows Form Designer generated code

        /// <summary>
        /// Required method for Designer support - do not modify
        /// the contents of this method with the code editor.
        /// </summary>
        private void InitializeComponent()
        {
            this.textBox1 = new System.Windows.Forms.TextBox();
            this.Udvozlo = new System.Windows.Forms.Label();
            this.button1 = new System.Windows.Forms.Button();
            this.Bevivo = new System.Windows.Forms.Label();
            this.Rogzito = new System.Windows.Forms.Button();
            this.SuspendLayout();
            // 
            // textBox1
            // 
            this.textBox1.Location = new System.Drawing.Point(15, 57);
            this.textBox1.Name = "textBox1";
            this.textBox1.Size = new System.Drawing.Size(196, 20);
            this.textBox1.TabIndex = 0;
            this.textBox1.TextChanged += new System.EventHandler(this.textBox1_TextChanged);
            // 
            // UdvozloCimke
            // 
            this.Udvozlo.ForeColor = System.Drawing.SystemColors.ControlText;
            this.Udvozlo.Location = new System.Drawing.Point(12, 10);
            this.Udvozlo.Name = "Udvozlo";
            this.Udvozlo.Size = new System.Drawing.Size(315, 36);
            this.Udvozlo.TabIndex = 1;
            this.Udvozlo.Text = "Üdvözöllek! Kérlek, írd be a keresendő fond nevét, vagy annak részletét és nyomd " +
    "meg a \'Keresés\' gombot!";
            this.Udvozlo.TextAlign = System.Drawing.ContentAlignment.MiddleCenter;
            this.Udvozlo.Click += new System.EventHandler(this.label1_Click);
            // 
            // KeresoGomb
            // 
            this.button1.Location = new System.Drawing.Point(231, 57);
            this.button1.Name = "Udvozlo";
            this.button1.Size = new System.Drawing.Size(96, 20);
            this.button1.TabIndex = 2;
            this.button1.Text = "Keresés";
            this.button1.UseVisualStyleBackColor = true;
            this.button1.Click += new System.EventHandler(this.button1_Click);
            // 
            // BevivoCimke
            // 
            this.Bevivo.Location = new System.Drawing.Point(15, 93);
            this.Bevivo.Name = "Bevivo";
            this.Bevivo.Size = new System.Drawing.Size(312, 36);
            this.Bevivo.TabIndex = 3;
            this.Bevivo.Text = "Ha új fondot szeretnél rögzíteni, kérlek, kattints az \'Új rögzítése\' gombra!";
            this.Bevivo.TextAlign = System.Drawing.ContentAlignment.MiddleCenter;
            this.Bevivo.Click += new System.EventHandler(this.label1_Click_1);
            // 
            // BevivoGomb
            // 
            this.Rogzito.BackgroundImageLayout = System.Windows.Forms.ImageLayout.None;
            this.Rogzito.Font = new System.Drawing.Font("Microsoft Sans Serif", 8.25F, System.Drawing.FontStyle.Regular, System.Drawing.GraphicsUnit.Point, ((byte)(238)));
            this.Rogzito.Location = new System.Drawing.Point(101, 142);
            this.Rogzito.Name = "Bevivo";
            this.Rogzito.Size = new System.Drawing.Size(141, 23);
            this.Rogzito.TabIndex = 4;
            this.Rogzito.Text = "Új rögzítése";
            this.Rogzito.UseVisualStyleBackColor = true;
            // 
            // Raktarkataszter
            // 
            this.AutoScaleDimensions = new System.Drawing.SizeF(6F, 13F);
            this.AutoScaleMode = System.Windows.Forms.AutoScaleMode.Font;
            this.ClientSize = new System.Drawing.Size(347, 195);
            this.Controls.Add(this.Rogzito);
            this.Controls.Add(this.Bevivo);
            this.Controls.Add(this.button1);
            this.Controls.Add(this.Udvozlo);
            this.Controls.Add(this.textBox1);
            this.Name = "Raktarkataszter";
            this.RightToLeft = System.Windows.Forms.RightToLeft.No;
            this.Text = "Raktarkataszter";
            this.Load += new System.EventHandler(this.Form1_Load);
            this.ResumeLayout(false);
            this.PerformLayout();

        }

        #endregion

        private System.Windows.Forms.TextBox textBox1;
        private System.Windows.Forms.Label Udvozlo;
        private System.Windows.Forms.Button button1;
        private System.Windows.Forms.Label Bevivo;
        private System.Windows.Forms.Button Rogzito;
    }
}
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Raktarkataszter
{
    public partial class Raktarkataszter : Form
    {
        public Raktarkataszter()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        {
           
        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void button1_Click(object sender, EventArgs e)
        {

        }

        private void label1_Click_1(object sender, EventArgs e)
        {

        }
    }
}
using System;
using System.Collections.Generic;
using System.Linq;
using System.Threading.Tasks;
using System.Windows.Forms;
using System.Data.OleDb;
using System.Diagnostics;
using System.IO;

namespace Raktarkataszter
{
    class Adatbazis
    {
  
    }
    class Faljkezelo
    {

    }
    static class Program
    {
        /// <summary>
        /// The main entry point for the application.
        /// </summary>
        [STAThread]
        static void Main()
        {
            
            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            StreamWriter a = new StreamWriter(@".\eleresiut.txt");
            if (File.Exists(@".\Raktar.accdb"))
            {
                OleDbConnection conn = new OleDbConnection();
            }
            else
            {
                Form a = new Form();
            }

            Application.Run(new Raktarkataszter());
            
           
        }
    }
}

