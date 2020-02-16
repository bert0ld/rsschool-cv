1. First Name, Last Name (real ones)
--
Anton Vanchin

2. Contact Info (add several ways to contact you)
--
Phone: +79101072000
VK: vk.com/vanish_xd
e-mail: vanishing9@yandex.ru

3. Summary (your goal, wishes, reveal what is important for you, what do you want and why.
Some kind of self-presentation. In case of lack of experience  Junior Developer sells his/her potential, his/her passion and ability to learn fast. You shouldn't think that everybody is going to teach you when you come to the workplace . Rather being a Junior means always
learning new things from everywhere etc.).
--
I'm really into self-education, self-improvement. It's my passion. Unfortunately it may be a reason to me not

4. Skills (e.g. programming languages, frameworks, methodologies, version control, tools etc.)
--
.......

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

6. Experience (for a Junior Dev it means all kinds of experience: coding tests, projects from courses,
freelance projects - wherever they had the opportunity to demonstrate skills they have.
Also it would be awesome if you add links to source code)
--
https://github.com/bert0ld
(I promise to add the university's projects.)


7. ***Education:***
* Studying in Nizhny Novgorod State University, 
Institute of Information Technologies, 
Mathematics and Mechanic (IITMM). 
Second-year student.

* Intel Delta 11 Course "Additional topics to the Software Engineering"

* [Data science marathon from Netology](https://netology.ru/programs/nauchite-iskusstvennyj-intellekt-pisat-scenarij-seriala?stop=1)

8. ***English***

Only studying practice in the university.
