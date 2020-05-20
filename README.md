# Video Banner Boilerplate

## Instructions
- Convert mp4 file to webm (https://convertio.co/mp4-webm/)
- Put videos on a CDN. I use s3 + Cloudfront for testing and then ask the client if they have a CDN to host the video on production (because video hosting is pretty costly).
- Use HTML5 video template
- Update banner dimensions in the following places
  - The ad.size meta tag (6)
  - The banner title tag (7)
  - The #animation_container div inline styles (148)
- Update video path to cdn path to video files (184)
- Update dates to change tune-in messaging based on date (188)
  - If only one tunein is provided, you can change the tune-in loader code in the loadTunein() function (270)
- Update video file names in the loadVideo() function (262)
- If social icons are needed:
  - uncomment socials in thml (168)
  - uncomment social vars (222, 223)
  - uncomment social visibility handlers (237, 243)
  - uncomment social event listeners (257-259)

## Things to Remember
- The file tree needs to remain flat, no folders allowed
- Remove any un-needed files before compressing/exporting
- Compress any image files when necessary (https://tinypng.com/)
- Try to keep the export size as small as possible
- The video size isn't added to the export size if served from an external cdn

## Resources
- [IAB Guidelines](https://www.iab.com/guidelines/)
- [IAB Digital Ads PDF](https://www.iab.com/wp-content/uploads/2016/04/HTML5forDigitalAdvertising2.0.pdf)
- [IAB Mobile Ads PDF](https://www.iab.com/wp-content/uploads/2015/11/IAB_Display_Mobile_Creative_Guidelines_HTML5_2015.pdf)
- [HTML5 Validator for DFP](https://h5validator.appspot.com/dcm)
- [Google Studio Enabler](https://www.google.com/doubleclick/studio/docs/sdk/html5/en/class_studio_Enabler.html)