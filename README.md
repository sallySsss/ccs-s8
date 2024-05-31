# ccs-s8
    // Функція, що повертає ім'я файлу для шифрування/розшифрування
    private string GetFileName()
    {
        if (Text == "")
        {
            do
            {
                if (saveFileDialog1.ShowDialog() == DialogResult.OK)
                {
                    Text = saveFileDialog1.FileName;
                    return saveFileDialog1.FileName;
                }
                else
                {
                    MessageBox.Show("Ви повинні створити або вибрати файл!");
                }
            } while (true);
        }
        else
        {
            return Text;
        }
    }
