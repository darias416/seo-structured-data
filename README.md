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
This code will produce a rich snippet containing a star rating and the name of the author that reviewed the product. 
```
<script type="application/ld+json">
{
  "@context": "https://schema.org/",
  "@type": "Product",
  "name": "",
  "image": "",
  "description": "",
  "sku": "",
  "mpn": "",
  "brand": {
    "@type": "Brand",
    "name": ""
  },
  "review": {
    "@type": "Review",
    "reviewRating": {
      "@type": "Rating",
      "ratingValue": "",
      "bestRating": ""
    },
"itemReviewed": {
     "@type": "Product",
     "image": "",
     "name": "",
"offers": {
    "@type": "Offer",
    "url": "",
    "priceCurrency": "",
    "price": "",
    "priceValidUntil": "2100-01-01",
    "itemCondition": "https://schema.org/NewCondition",
    "availability": "https://schema.org/OnlineOnly",
    "seller": {
      "@type": "Organization",
      "name": ""
    }
  }
    },
    "reviewBody": "",
    "author": {
      "@type": "Person",
      "name": ""
    },
    "publisher": {
      "@type": "Person",
      "name": ""
     },
  "offers": {
    "@type": "Offer",
    "url": "",
    "priceCurrency": "",
    "price": "",
    "priceValidUntil": "2100-01-01",
    "itemCondition": "https://schema.org/NewCondition",
    "availability": "https://schema.org/OnlineOnly"
    },
    "seller": {
      "@type": "",
      "name": ""
    }
  }
}
</script>
```
