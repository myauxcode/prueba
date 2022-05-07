
'PREGUNTA////////////////

 Public Function ejercicio6(n As Integer, vim As Double, m As Double, vi As Double, r As Double) As Double
        Dim f, t As Double
        vim = vim / m
        For i = 1 To n
            vim = vim * m
            t = vi + (r * (i - 1))
            f = f + (Math.Log10(vim) / t)

        Next
        Return f

    End Function

    Public Function ejercicio6t(n As Integer, vim As Double, m As Double, vi As Double, r As Double) As String
        Dim t As Double
        Dim s As String
        s = ""

        vim = vim / m
        For i = 1 To n
            vim = vim * m
            t = vi + (r * (i - 1))
            s = s + "(Log10(" + Str(vim) + ") / " + Str(t) + ")  +  "

        Next
        Return s

    End Function

'ENLACE///////////////

 TextBox6.Text = ejercicio6(TextBox1.Text, TextBox2.Text, TextBox3.Text, TextBox4.Text, TextBox5.Text)
  TextBox7.Text = ejercicio6t(TextBox1.Text, TextBox2.Text, TextBox3.Text, TextBox4.Text, TextBox5.Text)























