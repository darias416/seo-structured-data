# Structured Data Templates for Google Search

This repo contains a mix of structured data snippet templates that can be used to produce Rich Results via Google Search.

Snippets can be tested via Google's Rich Results test tool here: https://search.google.com/test/rich-results

Import Note: All structured data in this repo is optimized for affiliate review websites. Some of the structured data in this repo may yield "non-critical issue" warnings via the Rich Results test tool. These warnings can be ignored as the suggesstions made within these warnings are optional. 

# Contents:
**[Reviews](https://github.com/darias416/seo-structured-data/edit/main/README.md#reviews)**
- [Product Reviews](https://github.com/darias416/seo-structured-data/edit/main/README.md#product-reviews)

# Reviews
Structured data that will produce rich results for review articles.
## Product Reviews
This code will produce a rich snippet containing a star rating and the name of the author that reviewed the product. As of October 22, 2022, this code meets all of Google's requirements for Rich Snippets/Results and will not produce any warnings via the Rich Results test tool.
```
<script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Product",
      "name": "ENTER PRODUCT NAME HERE",
      "image": [
        "ENTER URL TO PRODUCT IMAGE HERE"
       ],
      "description": "ENTER PRODUCT DESCRIPTION HERE",
      "sku": "ENTER PRODUCT SKU HERE",
      "mpn": "ENTER PRODUCT MPN HERE",
      "brand": {
        "@type": "Brand",
        "name": "ENTER PRODUCT BRAND HERE"
      },
      "review": {
        "@type": "Review",
        "reviewRating": {
          "@type": "Rating",
          "ratingValue": "ENTER RATING HERE",
          "bestRating": "ENETER MAX POSSIBLE RATING HERE"
        },
        "author": {
          "@type": "Person",
          "name": "ENTER REVIEWER NAME HERE"
        }
      }
    }
    </script>
```
