# DRM_MPEGDASH  
**Digital Rights Management (DRM) for MPEG-DASH**  

This project demonstrates how to implement **DRM (Digital Rights Management)** for **MPEG-DASH** streams using encryption.  

## Features  
- **MPEG-DASH** streaming with DRM protection.  
- Includes a sample player using **Shaka Player**.  

## Prerequisites  
- **MP4Box** (for packaging and encryption)  
- **FFmpeg** (for media processing)  
- An **HTTPS server**  

## Directory structure
```
DRM_MPEGDASH/
├── README.md       
├── DRM_Multimedia_IgnacioMiguelRodríguez.pdf # Main documentation         
└── mpegdash/           # Example files
    ├── elephant/       # Elephant video data
    │   ├── output      # Encrypted segments 
    │   ├── elephant_drm.mpd     # DASH manifest
    │   └── elephant_drm.xml     # DRM XML
    ├── popeye/         # Popeye video data
    │   ├── output      # Encrypted segments 
    │   ├── popeye_drm.mpd     # DASH manifest
    │   └── popeye_drm.xml     # DRM XML
    ├── sintel/         # Sintel video data
    │   ├── output      # Encrypted segments 
    │   ├── sintel_drm.mpd     # DASH manifest
    │   └── sintel_drm.xml     # DRM XML
    ├── SourceSansPro-Regular.otf   # Font
    ├── generateXML.html  # Password-based XML generator page
    ├── index.html        # Home page
    ├── indexTest.html    # Demo HTML player
    ├── pbkdf2.js         # PBKDF2 function
    ├── server.pem        # HTTPS server's certificate
    └── server.py         # HTTPS server
```
## How to proceed  
### Encrypting streams and generating XML files
Note that these steps have already been performed. Only follow them if you want to change the password for encryption.
1. Access `generateXML.html` by clicking the Generate XML button on the home page.
2. Generate password-based XML for each video (note that this is already done).
3. Encrypt streams.
   
### Visualizing streams
1. Visualize streams by accessing `indexTest.html` by clicking the Visualize streams button on the home page.
2. Introduce the manifest path and password associated with that manifest.
3. Select the desired bitrate.


