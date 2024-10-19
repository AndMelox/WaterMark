# Image Watermarking Project

This project allows users to upload images and apply a watermark to them using a Node.js server. The server handles file uploads, processes the image, and returns the watermarked image to the client.

## Requirements

- Node.js (version 14 or higher)
- Docker

## Environment Variables

To run this project, you will need to add the following environment variables to your `.env` file or input them via console using the `comandos.txt` file.

### Discovery
`DISCOVERY_SERVICE_URL=http://192.168.2.194:6000`  
`LOAD_BALANCER_URL=http://192.168.2.194:4000`  
`MONITORING_SERVICE_URL=http://192.168.2.194:7000`  
`IP_ADDRESS=192.168.2.194`  
`SERVER_PORT=6000`

### Middleware
`DISCOVERY_SERVICE_URL=http://192.168.2.194:6000`  
`IP_ADDRESS=192.168.2.194`  
`PORT=4000`

### Dashboard
`SERVER_PORT=7000`  
`BASE_PORT=5000`  
`DISCOVERY_SERVICE_URL=http://192.168.2.194:6000`  
`HEALTH_CHECK_TIMEOUT=30000`  
`HEALTH_CHECK_INTERVAL=5000`  
`DOCKER_IMAGE_NAME=marcaagua`  
`IP_ADDRESS=192.168.2.168`

All these variables can be input directly by running the commands from the `comandos.txt` file in the console.

## Features

- Upload images in various formats (JPEG, PNG, BMP, TIFF).
- Convert WebP images to PNG format.
- Apply a watermark to the uploaded image.
- Resize the output image to a standard size (800x600 pixels).
- Ensures that both the watermark folder (`watermark`) and the image filenames are in lowercase for consistency.
- Supports cross-origin resource sharing (CORS) for easy integration with front-end applications.

## Technologies Used

- **Node.js**: JavaScript runtime for building the server.
- **Express**: Web framework for Node.js to handle HTTP requests.
- **Jimp**: Image processing library for handling image manipulation and watermarking.
- **Sharp**: High-performance image processing library for converting image formats.
- **Express-fileupload**: Middleware for handling file uploads in Express.
- **CORS**: Middleware to allow cross-origin requests.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AndMelox/WaterMark
   cd image-watermarking


## Authors

<img alt="GitHub" src="https://img.shields.io/badge/GitHub-@AndMelox-181717?style=flat-square&logo=github"> 
<img alt="GitHub" src="https://img.shields.io/badge/GitHub-@sebastian11020-181717?style=flat-square&logo=github">
<img alt="GitHub" src="https://img.shields.io/badge/GitHub-@SamVargasGit-181717?style=flat-square&logo=github">

## 🔗 Contact Links

<img alt="instagram" src="https://img.shields.io/badge/instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"> 
<img alt="linkedin" src="https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"> 
<img alt="gmail" src="https://img.shields.io/badge/gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"> 
<img alt="twitter" src="https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white"> ```
