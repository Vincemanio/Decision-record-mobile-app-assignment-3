# Content delivery network (CDN)

## Status
Proposed 

# context
Optimizing the delivery of content, particularly product images, is critical in the development of the new mobile app for the retail company. The motivation for this decision stems from the realization that the app will include a diverse range of product images of various sizes and resolutions. It is critical to efficiently deliver these images to users in order to ensure optimal app performance, quick loading times, and a seamless user experience.

## Decision
To improve the delivery of product images within the mobile app, we propose implementing a Content Delivery Network (CDN). A content delivery network (CDN) is a network of geographically distributed servers that stores cached copies of content, including images. When a user accesses the app, the CDN ensures that content such as product images are delivered from a server closest to the user's geographic location. This drastically reduces latency and speeds up image loading times. The CDN will also use image optimization techniques such as caching, lazy loading, and image compression. Caching will store frequently accessed images on edge servers, reducing the need to repeatedly retrieve the same images from the origin server. Lazy loading ensures that images are only loaded when they enter the user's viewport, conserving bandwidth and speeding up loading times. Image compression reduces image size while maintaining quality, resulting in improved performance.

## Consequences 
Users will notice faster image loading times, which will result in a smoother and more responsive app. Latency is reduced by delivering content from servers closer to users, improving the overall user experience. However, integrating a CDN necessitates careful selection of a reputable CDN service provider, consideration of data transfer and storage costs, and the implementation of caching policies. To maximize the benefits of this enhancement, the decision to use a CDN should be accompanied by efficient caching mechanisms within the app.


Decision record template by Michael Nygard



