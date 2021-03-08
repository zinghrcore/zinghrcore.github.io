# zinghrcore.github.io

## Portal NEWUX announcements https://zinghrcore.github.io/js/announcements.json

Following are the patterns for announcment.json.
Nnly single object is supported right now in main json array, although we can use **carousel** content type in order to provide multiple types of data

1. Image type

```
[{
  "startDate": "2021-01-20",
  "endDate": "2021-01-26",
  "isActive": true,
  "title":"", // title to show on popup header (optional)
  "caption": "", //caption to show after the content (optional)
  "url": "https://www.zinghr.com/", //url to redirect on click of content
  "type": "img/image",
  "mediaUrl":"url of image content",
  "img":"same as above(optional)"
}]
```

2. Video type <br/>
only playable video url supported, for embed contents e.g. youtube/facebook/twitter etc see next section

```
[{
  "startDate": "2021-01-20",
  "endDate": "2021-01-26",
  "isActive": true,
  "title":"", // title to show on popup header (optional)
  "caption": "", //caption to show after the content (optional)
  "url": "https://www.zinghr.com/", //url to redirect on click of content
  "type": "video",
  "mediaUrl":"url of video content",
  "video":"same as above(optional)"
}]
```

3. Embed type <br/>
This is basically iframe embed

```
[{
  "startDate": "2021-01-20",
  "endDate": "2021-01-26",
  "isActive": true,
  "title":"", // title to show on popup header (optional)
  "caption": "", //caption to show after the content (optional)
  "url": "https://www.zinghr.com/", //url to redirect on click of content
  "type": "embed",
  "mediaUrl":"url of iframe content"
}]
```
4. Html type <br/>
You can put some html content, if it is big content then iframe embeding is preferred
```
[{
  "startDate": "2021-01-20",
  "endDate": "2021-01-26",
  "isActive": true,
  "title":"", // title to show on popup header (optional)
  "caption": "", //caption to show after the content (optional)
  "url": "https://www.zinghr.com/", //url to redirect on click of content
  "type": "html",
  "htmlContent":"valid html content"
}]
```
5. Carousel type <br/>
in carousal type you can put all above contents in the form of sliders

```
[{
  "startDate": "2021-01-20",
  "endDate": "2021-01-26",
  "isActive": true,
  "title":"", // title to show on popup header (optional)
  "caption": "", //caption to show after the content (optional)
  "url": "https://www.zinghr.com/", //url to redirect on click of content
  "type": "carousel",
  "carouselContent":[<array-of-object-of-above-type-contents>]
}]
```
