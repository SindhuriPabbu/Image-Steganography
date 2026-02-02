# Image Steganography Tool

A simple GUI application built with Python and Tkinter that hides secret messages inside images using LSB (Least Significant Bit) steganography. Encode text into images or decode hidden messages with just a few clicks.

## ✨ Features
* Hide messages in PNG/JPG images using LSB technique
* Extract hidden messages from steganographic images
* User-friendly GUI with drag-and-drop simplicity
* No external server needed - runs completely offline
* Supports common image formats (PNG, JPG)

## 🛠️ Tech Stack
```
Python 3.x
├── tkinter (GUI)
├── Pillow (PIL) - Image processing
└── stegano - LSB steganography
```

## 📦 Installation
1. Clone/Download the repository
2. Install dependencies:
```
pip install pillow stegano
```
3. Run the application:
```
python steganography_gui.py
```

## 🚀 Quick Start
**Test images available!** Few sample images are provided in the `images/` folder to test the tool immediately.

1. Click "Open Image" to load your PNG/JPG file
2. Encode: Enter message → Click "Encode Message" (saves as stego_image.png)
3. Decode: Load any steganographic image → Click "Decode Message"
4. Use "Clear All" to reset

![Screenshot of the tool.](/images/steganography_tool.png "Tool Screenshot")
## 💡 How It Works
LSB Steganography replaces the least significant bits of image pixels with message bits:
```
Original pixel:  255, 128, 64  →  Encoded:  254, 129, 63
Message impact:  Invisible to human eye ✓
```
📁 File Structure
```
steganography_gui.py  # Main application
stego_image.png       # Output file (auto-generated)
```
⚠️ Limitations
* Works best with PNG images (lossless format)
* JPG may lose quality during encoding
* Message length limited by image size (~1KB per typical photo)

## 🔮 Future Enhancements
* Support for multiple file formats
* Password protection
* Batch processing
* Custom output filename
* Progress indicators

## 🤝 Contributing
1. Fork the repo
2. Create feature branch (git checkout -b feature/AmazingFeature)
3. Commit changes (git commit -m 'Add some AmazingFeature')
4. Push to branch (git push origin feature/AmazingFeature)
5. Open Pull Request

**Made with ❤️ for secure image messaging**
