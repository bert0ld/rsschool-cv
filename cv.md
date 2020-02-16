1. ***First Name, Last Name***

Anton Vanchin

2. ***Contact Info***

* Phone: +79101072000

* VK: vk.com/vanish_xd

* e-mail: vanishing9@yandex.ru

3. ***Summary***

I'm really into self-education, self-development directed to increasing the productivity. Following it I fell in love with running. Especially long distances like 10, 20 and more kilometers. And the closer I get to running a marathon, the more I understand the quote:

>Motivation is what gets you started. Habit is what keeps you going.

And i'm building a habit to study everyday and everywhere because even *small pause is a big chance to know something new*.

4. ***Skills***

*Languages:* 
* **C** and **C++** learned at the University and practiced there
* **MySQL** learned at the University with practiced there 
* **Pascal** learned at the School, had some practice during preparing to exam
* **C#(Windows Forms, .Net Framework 4.7.2)** learned at the University and practiced there

5. ***Code example***

C#, Windows Forms.
One of the university's task.
```c#
// Text editor
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;
using System.IO;

namespace TextEditor
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void OpenFile_Click(object sender, EventArgs e)
        {
            openFileDialog.Filter = "RTF files | *.rtf | Text files | *.txt | All files | *.*";

            if (openFileDialog.ShowDialog() == DialogResult.OK)
            {
                StreamReader sr = new StreamReader(openFileDialog.FileName);
                TextBox.Text = sr.ReadToEnd();
            }
        }

        private void SaveFile_Click(object sender, EventArgs e)
        {
            saveFileDialog.DefaultExt = "*.txt";
            saveFileDialog.Filter = "RTF files | *.rtf | Text files | *.txt | All files | *.*";

            if (saveFileDialog.ShowDialog() == DialogResult.OK && saveFileDialog.FileName.Length > 0)
            {
                StreamWriter sw = new StreamWriter(saveFileDialog.FileName);
                sw.WriteLine(TextBox.Text);
                sw.Close();
            }
        }

        private void NewFile_Click(object sender, EventArgs e)
        {
            TextBox.Clear();
        }

        private void boldbutton_Click(object sender, EventArgs e)
        {
            if (TextBox.SelectionFont != null)
            {
                Font CurrentFont = TextBox.SelectionFont;
                TextBox.SelectionFont = new Font(CurrentFont, CurrentFont.Style ^ FontStyle.Bold);
            }

            TextBox.SelectionLength = 0;
        }

        private void italicbutton_Click(object sender, EventArgs e)
        {
            if (TextBox.SelectionFont != null)
            {
                Font CurrentFont = TextBox.SelectionFont;
                TextBox.SelectionFont = new Font(CurrentFont, CurrentFont.Style ^ FontStyle.Italic);
            }

            TextBox.SelectionLength = 0;
        }

        private void fontdialogbutton_Click(object sender, EventArgs e)
        {
            FontDialog FD = new FontDialog();
            if (FD.ShowDialog() == DialogResult.OK)
            {
                TextBox.SelectionFont = FD.Font;
            }

            TextBox.SelectionLength = 0;
        }

        private void colordialogbutton_Click(object sender, EventArgs e)
        {
            ColorDialog CD = new ColorDialog();
            if (CD.ShowDialog() == DialogResult.OK)
            {
                TextBox.SelectionColor = CD.Color;
            }

            TextBox.SelectionLength = 0;
        }

        private void UndoTextTool_Click(object sender, EventArgs e)
        {
            TextBox.Undo();
        }

        private void RedoTextTool_Click(object sender, EventArgs e)
        {
            TextBox.Redo();
        }

        private void CutTextTool_Click(object sender, EventArgs e)
        {
            TextBox.Cut();
        }

        private void CopyTextTool_Click(object sender, EventArgs e)
        {
            TextBox.Copy();
        }

        private void PasteTextTool_Click(object sender, EventArgs e)
        {
            TextBox.Paste();
        }
    }
}
```

6. ***Experience***

https://github.com/bert0ld
>I promise to add the university's projects.


7. ***Education:***
* Studying in Nizhny Novgorod State University, 
Institute of Information Technologies, 
Mathematics and Mechanic (IITMM). 
Second-year student.

* Intel Delta 11 Course "Additional topics to the Software Engineering"

* [Data science marathon from Netology](https://netology.ru/programs/nauchite-iskusstvennyj-intellekt-pisat-scenarij-seriala?stop=1)

8. ***English***

Only studying practice in the university.
