# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_view",
  "detailed_event": "Page Load Started",
    "page_data": {
        "affiliate_id": "<affiliate_id>",
        "breadcrumb": "<breadcrumb>",
        "country": "<country>",
        "language": "<language>",
        "owner": "<owner>",
        "page_location": "<page_location>",
        "site_section": "<site_section>",
        "site_section2": "<site_section2>",
        "site_type": "<site_type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.affiliate_id|string|Captures the ID of the affiliate related to a given event||||||||
|page_data.breadcrumb|string|A delimited list of hierarchical sections that describe the current page's location within the navigation of the site.|Home&gt;Women&gt;Tops&gt;Sweaters, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Checkout &gt; Order Thank You|||||||
|page_data.country|string|The country the site is associated with.||||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.||||||||
|page_data.owner|string|Captures the licensee or owner of content \(i.e. HBO\).|XX product management, marketing, vendor name|||||||
|page_data.page_location|string|The url of the page currently being viewed.||||||||
|page_data.site_section|string|The section of the site that the current page resides in. site\_section2 through site\_section5can also be used if the site has many sections.||||||||
|page_data.site_section2|string|Captures the sub-section of the site where the page being viewed is located|Shop &gt; Kids, Shop &gt; Mens, Shop &gt; Womens|||||||
|page_data.site_type|string|Common language description of the site type of purpose. May be used to group siteName.|Prospecting, Shop, Members, Brand|||||||




