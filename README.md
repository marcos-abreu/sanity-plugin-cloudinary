# Sanity + Cloudinary =	🖼️

## Installation

`sanity install cloudinary`

## Usage

Declare a field to be `cloudinary.asset` in your schema

```javascript
     /...,
    {
      type: "cloudinary.asset",
      name: "image",
      description: "This asset is served from Cloudinary",
    }
```

Uses Cloudinary media library for selecting assets and transformations

<img width="1416" alt="Screen Shot 2021-03-22 at 10 33 58 PM" src="https://user-images.githubusercontent.com/38528/112098236-b41e3f80-8b5e-11eb-9ee2-aa243420cf03.png">


<img width="996" alt="Screen Shot 2021-03-22 at 10 07 52 PM" src="https://user-images.githubusercontent.com/38528/112096210-0f4e3300-8b5b-11eb-9f26-45481df878ba.png">

## Content
Here is an example of which data is stored on your documents after selecting an asset.

```json
{
    "public_id": "29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x",
    "resource_type": "image",
    "type": "upload",
    "format": "jpg",
    "version": 1616474653,
    "url": "http://res.cloudinary.com/dzwiku20l/image/upload/v1616474653/29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x.jpg",
    "secure_url": "https://res.cloudinary.com/dzwiku20l/image/upload/v1616474653/29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x.jpg",
    "width": 2400,
    "height": 1344,
    "bytes": 547710,
    "duration": null,
    "tags": [],
    "metadata": {},
    "created_at": "2021-03-23T04:44:13Z",
    "access_mode": "public",
    "_version": 1,
    "_type": "cloudinary.asset"
  }
```

## Transformations

You can create a transformation when selecting the asset, and this information is previewed and stored

<img width="915" alt="Screen Shot 2021-03-22 at 10 37 27 PM" src="https://user-images.githubusercontent.com/38528/112098534-30b11e00-8b5f-11eb-8a42-d4674d013148.png">

```json
{
    "public_id": "29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x",
    "resource_type": "image",
    "type": "upload",
    "format": "jpg",
    "version": 1616474653,
    "url": "http://res.cloudinary.com/dzwiku20l/image/upload/v1616474653/29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x.jpg",
    "secure_url": "https://res.cloudinary.com/dzwiku20l/image/upload/v1616474653/29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x.jpg",
    "width": 2400,
    "height": 1344,
    "bytes": 547710,
    "duration": null,
    "tags": null,
    "metadata": [],
    "created_at": "2021-03-23T04:44:13Z",
    "derived": [
      {
        "url": "http://res.cloudinary.com/dzwiku20l/image/upload/a_45/v1616474653/29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x.jpg",
        "secure_url": "https://res.cloudinary.com/dzwiku20l/image/upload/a_45/v1616474653/29b4a88182b4cb50330011d23a29bcb371bd5886-2400x1344_lzcx7x.jpg",
        "raw_transformation": "a_45"
      }
    ],
    "access_mode": "public",
    "_version": 1,
    "_type": "cloudinary.asset"
  }
```

## Video

Video assets gets a video player preview in the Studio

<img width="709" alt="Screen Shot 2021-03-22 at 10 42 04 PM" src="https://user-images.githubusercontent.com/38528/112098938-d49ac980-8b5f-11eb-8c1f-fb269ac289cf.png">

```json
{
    "public_id": "Make_it_happen_together.-WWa8qtgD0f0_nucpr9",
    "resource_type": "video",
    "type": "upload",
    "format": "mp4",
    "version": 1616474928,
    "url": "http://res.cloudinary.com/dzwiku20l/video/upload/v1616474928/Make_it_happen_together.-WWa8qtgD0f0_nucpr9.mp4",
    "secure_url": "https://res.cloudinary.com/dzwiku20l/video/upload/v1616474928/Make_it_happen_together.-WWa8qtgD0f0_nucpr9.mp4",
    "width": 1920,
    "height": 1080,
    "bytes": 3937717,
    "duration": 24.1,
    "tags": [],
    "metadata": [],
    "created_at": "2021-03-23T04:48:48Z",
    "access_mode": "public",
    "_version": 1,
    "_type": "cloudinary.asset"
  }
```
