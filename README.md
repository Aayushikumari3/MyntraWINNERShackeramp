# MyntraWINNERShackeramp
3D try on for everything:
HOW VIRTUAL TRY-ON TECHNOLOGY WORKS
Virtual try-on technology employs computer vision and machine learning algorithms to enable users to visualize how a particular product, such as clothing, eyewear, or makeup, would appear on them without the need for physical trials. On the basic level, these solutions can be found in AR frameworks like Apple’s ARKit & RealityKit or Google’s ARCore so we can use them without the involvement of AI specialists. For example,  ARCore integrates the virtual and the real using the three vital features of a smartphone’s camera: motion-tracking, environmental understanding, and light estimation.

Some solutions allow users to observe the product on themselves in real-time as they move and interact with the system. These rely on a live video feed from the user’s camera and employ computer vision algorithms to track the user’s actions, continuously updating the virtual try-on display.

In contrast, non-real-time virtual try-on solutions allow users to upload a photo or video of themselves and then view how the product would look on them in a static image or video format. This approach does not necessitate a live video feed and is useful in scenarios where real-time interaction is unnecessary or impractical, such as on e-commerce product pages or at in-store kiosks.

Each real-time and non-real-time virtual try-on solution has its own unique merits and drawbacks, with the choice depending on the specific application and use case. Real-time solutions offer a more immersive and engaging experience, whereas non-real-time virtual try-on solutions are better suited for situations where real-time interaction is not essential.

VIRTUAL TRY-ON SOLUTIONS OVERVIEW
The virtual try-ontechnology market provides offerings for accessories, watches, glasses, hats, clothes, and more. Some types of solutions can be developed with AR frameworks like ARKit and ARCore, but when it comes to more complex cases, we might face the limitations of these tools. Judging from our experience, ARKit is good enough for the simplest facial recognition architecture. For more advanced projects, we need to use AI to meet specific goals, for example, segmentation of face and hair in case we want to create a virtual try-on with various hair colors. From a technological point of view, virtual try-on projects might require AR technology for basic visualization and additional AI technology for calculations. 

VIRTUAL TRY-ON FOR WATCHES
When it comes to virtual try-on watches, the capabilities of ARKit/ARcore might seem limited to demonstrating the best results, as ARKit recognizes the body as one unit, and ARCore doesn’t have built-in body recognition at all. So, in most cases, we will need to use additional AI expertise and/or utilize ready-to-use hand recognition models for tracking and recognition. 

An interesting example of a virtual watch try-on is the AR-Watches app which allows users to try on various watches. The solution is based on the AR Markers utilizing specific markers printed on a band, which should be worn on a user’s wrist in place of a watch in order to start a virtual try-on with the watch. The computer vision algorithm processes only those markers visible in the frame and identifies the camera’s position in relation to them to render a 3D object correctly. Of course, technology has its limits (for instance, not everybody has a printer at hand to print out the AR Markers band). But if it matches the business use case, it wouldn’t be that difficult to create a product with a production-ready quality. Probably, the most important part would be to create proper 3D objects to use.

VIRTUAL TRY-ON FOR SHOES
For virtual try-on shoes, we also need to use pose estimation models, in this case, foot estimation models. This task is more specific than hand estimation as it’s rarer, so in some cases, such solutions will require creating and training your own models. 

Technically, a virtual try-on solution for shoes utilizes a foot pose estimation model based on deep learning. This technology may be considered for a particular case of widespread full-body 3D pose estimation models that estimate the position of selected keypoints in the 3D dimension directly or through the inference of detected 2D keypoints’ positions into 3D coordinates.

Once positions of 3D keypoints of feet are detected, they can be utilized for creating a parametric 3D model of a human foot, and positioning & scaling of a footwear 3D model according to the geometric properties of the parametric model.

Positioning of a 3D model of a footwear on top of a detected parametric foot model
Positioning of a 3D model of footwear on top of a detected parametric foot model (source)

Compared to the full-body/face pose estimation model, foot pose estimation still has certain challenges. The main issue is the lack of 3D annotation data required for model training. 

However, the optimal way to avoid this problem is to use synthetic data, which supposes rendering of photorealistic 3D human feet models with key points and training a model with that data.  You can also opt to use photogrammetry which supposes the reconstruction of a 3D scene from multiple 2D views to decrease the number of labeling needs.

This kind of solution is way more complicated. In order to enter the market with a ready-to-use product, it is required to collect a large enough foot keypoint dataset (either using synthetic data, photogrammetry, or a combination of both), train a customized pose estimation model (that would combine both high enough accuracy and inference speed), test its robustness in various conditions and create a foot model. We consider it a medium-complexity project in terms of technologies.

Lines
Read also:
Using Human Pose Estimation in Fitness & Rehab Therapy Apps
VIRTUAL TRY-ON FOR GLASSES
FittingBox and Ditto’s companies considered AR technology for virtual glasses try-on. The user should choose a glasses model from a virtual catalog and it is put on his/her eyes.

This solution is based on the deep learning-powered pose estimation approach utilized for facial landmarks detection, where the common annotation format includes 68 2D/3D facial landmarks.

Such an annotation format allows the differentiation of face contour, nose, eyes, eyebrows, and lips with a sufficient accuracy level. The data for training the face landmark estimation model might be taken from such open-source libraries as Face Alignment, providing face pose estimation functionality out-of-the-box.

In terms of technologies, this kind of solution is not that complicated, especially if using any pre-trained model as a basis for the face recognition task. Therefore, such solutions can be developed with existing AR frameworks like ARKit/ARcore for the most basic features. A more sophisticated approach will require additional AI expertise as well. It’s important to consider that low-quality cameras and poor light conditions could be limiting factors in that regard.

VIRTUAL TRY-ON FOR HATS
As facial landmark detection models work well, another frequently simulated AR item is hats. All that is  required for the correct rendering of a hat on the person’s head is the 3D coordinates of several keypoints indicating temples and the location of a forehead center. The basic types of these solutions usually can be developed with AR frameworks.

VIRTUAL TRY-ON FOR FURNITURE
Virtual try-on for furniture is increasingly becoming a valuable tool for both retailers and customers in the furniture industry, as it bridges the gap between online and physical shopping experiences and offers a more informed and satisfying purchasing process. The technology enables real-time visualization, allowing customers to move, rotate, and place virtual furniture within their physical environment. They can view the furniture from different angles and in various positions. 

Customers can adjust the size and scale of virtual furniture items to ensure they fit perfectly within their space. This helps prevent issues related to furniture that is too large or too small for a room. Some virtual try-on platforms allow users to customize furniture items by selecting different colors, materials, and finishes to match their preferences and decor.

Here, we need to understand the limitations of technology as virtual try-on furniture doesn’t show the best results with AR technology in real-time. It usually requires the involvement of AI technology and more time to adjust the new furniture, for example, to match existing furniture in the room. Such projects require more resources, expertise, and time to develop. 

MAKEUP VIRTUAL TRY-ONS
Makeup virtual try-ons have gained popularity among beauty enthusiasts and shoppers, revolutionizing the way makeup products are selected and purchased. They provide a fun and informative way to explore makeup options, experiment with new looks, and make informed choices when shopping for cosmetics.

Users can experiment with makeup looks either in real-time using their device’s camera or by uploading photos/videos. Real-time mode enables users to see themselves wearing the virtual makeup as they move and interact. Some virtual try-ons offer makeup tutorials and beauty tips to guide users in achieving specific looks or makeup styles. An excellent example is L’Oreal’s solution which allows customers to see how different colors of lipstick, mascara, eyeshadow, and foundation will look on them before they make a purchase. 

Such solutions usually require AI technology in addition to AR frameworks to segment the face zones. We can use ready-to-use models for this use case for the most basic features.

VIRTUAL TRY-ON FOR CLOTHES
Virtual fitting room technology enables customers to use their camera-equipped devices within a dedicated app. Through this app, customers can explore products in detail. These models can be overlaid onto the customer’s own image, helping them assess the suitability of a product, including the ability to measure their body and recommend the most appropriate size. This interactive experience aids customers in making informed purchase decisions.

Compared to shoes, masks, glasses, and watches, developing virtual try-on 3D clothing solutions is a more challenging task. The reason for that is simple: clothes are deformed when taking the shape of a person’s body. Thus, for a proper AR experience, a deep learning model should identify not only basic keypoints on the human body’s joints but also the body shape in 3D. There already are models for pose estimation and body segmentation that can meet business needs. 

However, sometimes, the keypoints they offer might be not enough for specific tasks, for example, when it comes to underwear. In this case, we will need to develop custom models for specific tasks. Here, the type of virtual try-on solutions makes a difference too. When we talk about a “magic mirror” in a store, it might be easier as we have a fixed camera with a fixed angle for capturing the image. In the case of smartphones and tablets, the task becomes more difficult as the position of the camera might change and the pose estimation is way more challenging. 

Lines
Read also:
Virtual Fitting Room Development Using AR & AI Technologies
VIRTUAL TRY-ON FOR PETS
A virtual try-on for pets allows pet owners to virtually try on various products, such as clothing, accessories, or even grooming styles, on images or videos of their pets. This technology leverages augmented reality (AR) or computer vision to overlay and visualize these products on the pet, giving the owner an idea of how the item would look on their furry companion.

For example, in 2021, online pet supply retailer Chewy offered an exciting product for four-legged friends with their “Fur-tual Boutique” virtual try-on experience. Dogs and cats virtually try out seven of Chewy’s most popular Halloween costumes from Frisco, including Cowboy, Killer Doll, Granny and Superhero.

Such applications often employ technologies like image recognition, object tracking, and AR to accurately overlay and visualize the products on the pet images or videos.

WHAT TO CONSIDER BEFORE DEVELOPING A VIRTUAL TRY-ON APP
Although virtual try-on apps have gradually become the new standard of customer experience, creating such solutions may come with some challenges. From a technological point of view, there are some aspects to pay attention to. 

First of all, we don’t provide ready-to-use solutions. We use our technological expertise and experience as the foundation of a custom product which is more flexible and less expensive in the long term. This is very true if you consider that you usually need to pay on a regular basis for ready-to-use solutions. 

The most common challenges while building custom virtual try-on solutions include the following: 

Optimizing application performance
To ensure optimal performance, certain constraints must be applied to your solution. For instance, when dealing with video, maintaining a stable rate of at least 25 frames per second is essential. The demands are somewhat more tolerant for image processing, but it’s crucial to keep user waiting times to no more than a second or two.

When addressing performance, predicting how the app will function across different devices can be challenging. The best approach involves testing the final application on a range of devices beyond just sophisticated phones.

While leveraging cloud computing may seem appealing due to its virtually limitless processing power for a virtual try-on app, there are significant drawbacks. Firstly, the app becomes highly reliant on a fast internet connection. Temporary slowdowns can lead to a less responsive user experience, potentially discouraging users.

Securing data privacy
Another critical concern is data privacy, a growing issue in today’s digital landscape. Modern app users are increasingly conscious of their data privacy. Moreover, sharing photos or videos, particularly when it involves items like tight-fitting clothing, can raise privacy concerns. To meet compliance requirements it’s necessary to implement an appropriate consent mechanism to allow users to give consent to use their data. 

Although cloud computing opens up new opportunities for development, it also introduces potential security vulnerabilities that require extra precautions and expertise to ensure data security. A simpler, and potentially safer, solution is to perform computations directly on the user’s device.

Creating 3D models
Obtaining high-quality 3D models is crucial for the success of your virtual try-on application. Several approaches can be taken to tackle this challenge. One option is to invest in a dedicated 3D scanner with accompanying software to generate top-tier models. Alternatively, you can hire a skilled 3D artist to create the models. Whatever you choose, it comes with additional costs for design. 

It’s essential to prepare these 3D models in advance, as the conversion of photos into 3D models may require 20-40 minutes using algorithms. Additionally, the models should be stored in a cloud and downloaded onto the end user’s device as needed, as they can be quite large in size.

Consider offering models in two quality levels – low and high. The low-quality model is lightweight and can be quickly downloaded and presented to the user. Meanwhile, the higher-quality model can be downloaded in the background and swapped when ready. 

Overall, you should remember that developing a try-on solution requires a high level of technical expertise to ensure the quality of the final product. It’s also important to have realistic expectations for your future product and understand the limitations of the technology. 

CASE STUDY: FACE CARE PRODUCT TRY-ON SOLUTION FOR A COSMETIC BRAND
The business wanted to improve user engagement on the site and decided to create a try-on cosmetics solution to achieve the goal. With this solution, we needed to demonstrate how to apply face care products to educate and entertain customers. 

From a technological point of view, we decided to use animation as the best option for this case.  We created a specific algorithm for showing and binding animations to a face which consisted of several parts. 

1.Detecting zones to apply the cosmetics

Any human face has face landmarks:

Landmark set with the primary landmarks
Landmark set includes squares representing the primary (first order) landmarks (source)

We found them on the displayed face using a previously trained neural network (dataset with 35,000 faces). Its architecture was adapted to work in the browser in real-time (Tiny Face Landmarks 68).

Knowing the coordinates of the face landmarks, we defined the coordinates of the critical zones of the face relative to the nearest landmarks. Relative to the convex polygon — which was described by the carrier points of the critical zone — a place was determined where the cosmetics should be applied. Accordingly, it was necessary to show the animation for the “how to use” zone. Since the coordinates of the face landmarks were continuously changing over time, we needed to superimpose the pattern of the critical zone.

We draw a horizontal rectangle (bounding box) around the convex polygon so that the distant vertices of the polygon lie on the edges of the rectangle.

How to determine the bounding box
Since we didn’t need scientific accuracy, it was enough to sort the face landmark coordinates vertically and horizontally — and took their extreme values to determine the bounding box. This is how we got a rectangle with the critical area for applying the cosmetic product. This was the area we needed to animate.

 If we changed the face landmark coordinates, the critical zone and the bounding box coordinates would change proportionally.

2. Working with animation

Using this approach, we drew an animation on a rectangular fragment of the HTML5 canvas of the original size. Afterward, we superimposed the animation on the image, having changed the scale according to the new coordinates of the bounding box.

Since we used a simplified algorithm and converted 3D coordinates to 2D, there could be superimposition artifacts. So, we offered to make the following possible improvements to the algorithm:

Use of the non-horizontal bounding box
Use of an improved face landmark determination engine, which can provide 3D coordinates
As these improvements take additional time for the development of more resource-consuming algorithms, we decided to implement them at the later stages of development. 

3. Synchronizing the animation with the calculation of the face landmark coordinates

We should also note another issue: synchronization of the animation with the calculation of the face landmark coordinates. Depending on the device type (mobile/desktop), operating system, memory, processing power, and other conditions, the performance of the neural network may change significantly. This is why we needed to sync the animation with the time required by the neural network to determine the face landmarks. For that purpose, we needed to know the number of milliseconds between frames. Then we calculated the new position of the animated zone based on this value. Thus, the animation on low-performance devices still may lag, however, it would maintain the synchronization with the position of the key face landmarks.

CHALLENGES OF THE PROJECT AND ADDITIONAL REMARKS 
The neural network (FaceLandmarks 68) didn’t contain the key point for the upper point of the forehead. However, there might be a need to apply cosmetics to the forehead as well. To solve this problem and find the upper point of the forehead, we needed to know that the key user audience of our app is adult women, whose face proportions are known beforehand.

Knowing the position of the face landmarks for the lower point of the chin and the upper points of the eyebrows, it was possible to calculate the coordinates for the top of the forehead. Thus we were able to build a carrier triangle, which would later be used to build the bounding box for the forehead zone.

Since the algorithm described above didn’t contain critical restrictions regarding the animation, it was possible to use a heat map to indicate the zones where thicker layers of cosmetics should be applied, as shown in the image below. We suggested implementing the functionality with face-api.js or brfv5-browser.

The same algorithm could be used to display animations over a selfie or a photo of the model. The only difference is that since there was no need for real-time calculations (the face image is static), the landmarks were calculated only once, at the start of the animation. In addition, since the calculation was performed only once, it was possible to improve accuracy by using the fully functional FaceLandmark68 neural network instead of TinyFaceLandmark68 (which was adapted for real-time calculations).

For such cases, there is a video with animation prepared beforehand. This reduces the in-browser calculations and expands the user audience to low-performance devices. 
