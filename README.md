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
