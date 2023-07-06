https://apify.com/epctex/tiktok-video-downloader

# Actor - Tiktok Video Downloder

## Tiktok Video Downloder

Since Tiktok  doesn't provide a good and free API, this actor should help you to download data from it.

The Tiktok Video Downloder supports the following features:

-   Download Video - If you want to get videos on a certain URL ,just type the url.

## Bugs, fixes, updates and changelog

This video downloader is under active development. If you have any feature requests you can create an issue from [here](https://github.com/epctex/tiktok-video-downloader/issues).


## Input Parameters

The input of this video downloader should be JSON containing the list of pages on Tiktok that should be visited. Required fields are:

- `startUrls`: (Optional) (Array) List of Tiktok URLs. You should only provide detail URLs

- `proxy`: (Required) (Proxy Object) Proxy configuration.

- `extendOutputFunction`: (Optional) (String) Function that takes a JQuery handle ($) as argument and returns object with data.

- `customMapFunction`: (Optional) (String) Function that takes each objects handle as argument and returns object with executing the function.

This solution requires the use of **Proxy servers**, either your own proxy servers or you can use [Apify Proxy](https://www.apify.com/docs/proxy).

### Tip

When you want to have a scrape over a specific list URL, just copy and paste the link as one of the **startUrl**

### Compute Unit Consumption

The actor optimized to run blazing fast and scrape as many items as possible. Therefore, it forefronts all the detail requests. If actor doesn't block very often it'll scrape 1 video in under 45 seconds with ~0.01-0.02 compute units.

### Tiktok video downloader Input example

```json
{
    "startUrls": [

    ],
    "proxy": {
        "useApifyProxy": true
    }
}
```

## During the Run

During the run, the actor will output messages letting you know what is going on. Each message always contains a short label specifying which page from the provided list is currently specified.
When items are loaded from the page, you should see a message about this event with a loaded item count and total item count for each page.

If you provide incorrect input to the actor, it will immediately stop with failure state and output an explanation of what is wrong.

## Tiktok Export

During the run, the actor stores results into a dataset. Each item is a separate item in the dataset.

You can manage the results in any languague (Python, PHP, Node JS/NPM). See the FAQ or <a href="https://www.apify.com/docs/api" target="blank">our API reference</a> to learn more about getting results from this Tiktok Video downloader.

## Downloaded Tiktok Properties

The structure of each item in Tiktok looks like this:

### Item Detail

```json
{
	"title": "Web scraping meets geography 🗺️#googlemaps #webscraping #dataextraction #geolocation #coordinates #api #data",
	"sourceUrl": "https://www.tiktok.com/@apifytech/video/7231446296006020379",
	"downloadUrl": "https://api.apify.com/v2/key-value-stores/04e889f7-a2c2-4ed3-ad68-e27c9700e68c/records/7231446296006020379"
}
```

## Contact 
Please visit us through [epctex.com](https://epctex.com) to see all the products that is available for you. If you are looking for any custom integration or so, please reach out to us through the chat box in [epctex.com](https://epctex.com). In need of support? [devops@epctex.com](mailto:devops@epctex.com) is at your service.
