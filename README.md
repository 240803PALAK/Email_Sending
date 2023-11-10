# Email_Sending


    import smtplib as s
    ob=s.SMTP('smtp.gmail.com',587)
    ob.ehlo()
    ob.starttls()
    ob.login('your@gmail.com','password')
    subject="test python"
    body="I love Python"
    massage="subject:{}\n\n{}".format(subject,body)
    listadd=['sender@gmail.com','sender@gmail.com']
    ob.sendmail('palakarahandale@gmail.com',listadd,massage)
    print('Send mail')
    ob.quit()
