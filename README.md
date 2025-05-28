Public Class Form1


    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        Close()
    End Sub

    Private Sub btnSubmit_Click(sender As Object, e As EventArgs) Handles btnSubmit.Click
        'Variables:
        Dim decMessage1 As Decimal

        Dim decres1 As Decimal
        Dim decres2 As Decimal
        Dim decres3 As Decimal

        'Gather inputs:
        decMessage1 = txtMessage.Text

        'Do Calculations:
        decres1 = decMessage1 * 0.7
        decres2 = decMessage1 * 0.2
        decres3 = decMessage1 * 0.1

        'Display Outputs:
        lbl1.Text = decres1
        lbl2.Text = decres2
        lbl3.Text = decres3



    End Sub

    Private Sub btnClear_Click(sender As Object, e As EventArgs) Handles btnClear.Click
        txtMessage.Clear()

        lbl1.ResetText()
        lbl2.ResetText()
        lbl3.ResetText()

        txtMessage.Focus()
    End Sub


End Class
