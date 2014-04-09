Slide-Up-Animation
==================

' Slide up animation for VB.NET

     If PictureBox13.Location.Y >= 155 Then
            TwitterGoUp.Enabled = False
        Else

            'Initial Location of all items
            Dim loc As Integer
            Dim Loc2 As Integer
            Dim Loc3 As Integer
            Dim Loc4 As Integer
            loc = PictureBox13.Location.Y + 10
            Loc2 = Label10.Location.Y + 10
            Loc3 = Button1.Location.Y + 10
            Loc4 = LinkLabel1.Location.Y + 10

            Loc2 = loc - 10
            If PictureBox13.Location.Y >= 155 Then

                'Visible After Animation
                Label26.Visible = False
                LinkLabel7.Visible = False
                LinkLabel8.Visible = False
                LinkLabel9.Visible = False

                ' Disable the Animation
                AnimationFacebook.Enabled = False

            Else
                PictureBox13.Location = New Point(84, loc)
                Label10.Location = New Point(8, Loc2)
                Button1.Location = New Point(114, Loc3)
                LinkLabel1.Location = New Point(82, Loc4)
            End If
        End If
