---
title: Qr Code Generator
---
```py
import qrcode

def create_qrcode(data, filename):
    qr = qrcode.QRCode(
        version=1,
        error_correction=qrcode.constants.ERROR_CORRECT_L,
        box_size=10,
        border=4,
    )
    qr.add_data(data)
    qr.make(fit=True)

    img = qr.make_image(fill_color="black", back_color="white")
    img.save(filename)

# Example usage
data = ""
filename = "qrcode.png"
create_qrcode(data, filename)
```