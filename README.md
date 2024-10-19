# Image Watermarking Project

This project allows users to upload images and apply a watermark to them using a Node.js server. The server handles file uploads, processes the image, and returns the watermarked image to the client.

## Requirements

- Node.js (version 14 or higher)
- Docker

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file:

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

## Features

- Upload images in various formats (JPEG, PNG, BMP, TIFF).
- Convert WebP images to PNG format.
- Apply a watermark to the uploaded image.
- Resize the output image to a standard size (800x600 pixels).
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
   git clone https://github.com/yourusername/image-watermarking.git
   cd image-watermarking
   