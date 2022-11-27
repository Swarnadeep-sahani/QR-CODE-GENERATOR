![information](https://user-images.githubusercontent.com/108685284/204118652-67dc26bb-4869-48de-9359-1a483a3fa0a4.png)
# QR-CODE-GENERATOR

import qrcode

import image

qr=qrcode.QRCode(
    version=15,
    box_size=10,
    border=5
    )
data="MY NAME IS SWARNADEEP SAHANI AND I AM A BTECH 2ND YEAR STUDENT"
qr.add_data(data)
qr.make(fit=True)
img=qr.make_image(fit="black",back_color="white")
img.save("information.png")
