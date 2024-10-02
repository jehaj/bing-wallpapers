# bing-wallpapers
Download bing wallpapers.

## Finding the source
Calling `https://www.bing.com/hp/api/v1/imagegallery?format=json&ssd=20241002_0700&wlexpsignin=1` gives JSON with 7 different images (up to UHD when landscape). They are at `data.images[].imageUrls.landscape.ultraHighDef`.

So either run daily or weekly to add images.

## Understanding it
Use Jq with `.data.images[].imageUrls.landscape.ultraHighDef` to get the path of images.
