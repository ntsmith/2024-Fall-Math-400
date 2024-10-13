# Use an official Node.js image as the base
FROM node:lts-slim

# Install required system dependencies, including Chromium and dependencies for running it in a container
RUN apt-get update && \
    apt-get install -y \
    pandoc texlive-full git \
    libasound2 libatk-bridge2.0-0 libatk1.0-0 libcups2 libdbus-1-3 \
    libdrm2 libgbm1 libgtk-3-0 libnspr4 libnss3 libxcomposite1 libxdamage1 \
    libxrandr2 xdg-utils libu2f-udev libvulkan1 libwayland-client0 libwayland-server0 \
    libxshmfence1 libx11-xcb1 libxcb-dri3-0 libgbm-dev chromium \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Install md-to-pdf globally using npm

RUN npm install -g md-to-pdf

USER node

RUN npx puppeteer browsers install chrome

# Set up the working directory in the container
WORKDIR /workspace

# # Expose port 3000 (if needed for testing or running other services)
# EXPOSE 3000

# # Define an entrypoint (optional, can be overridden later) 
# ENTRYPOINT ["md-to-pdf"]

# # CMD for running md-to-pdf (optional, can be overridden)
# CMD ["--help"]
