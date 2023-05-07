
# I haven't watched the whole video yet, but I have an opinion about it
The emergence of social media platforms has brought about both opportunities and challenges, particularly with regards to user engagement and communication. This study focuses on analyzing the variance between early and steady state responses to political overtones on YouTube. The objective is to investigate the difference between comments made by users before and after the midpoint of the video, based on comment timestamps, video timestamps, and duration. Natural Language Processing (NLP) techniques will be employed to classify comments as either early or steady state responses, and to extract meaningful insights from the data. This research aims to contribute to a better understanding of user engagement and communication on social media platforms, particularly in the context of political discourse.
## Roadmap

- Data Extraction 

- Classification comments as steady state and early responses


## Authors

- [@Ashique Khudabuksh](https://www.github.com/octokatherine)
- [@SaiTulasi Kamma](https://www.github.com/octokatherine)


## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### add(num1, num2)

Takes two numbers and returns the sum.


## Appendix

Any additional information goes here


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)

## Color Reference

| Color             | Hex                                                                |
| ----------------- | ------------------------------------------------------------------ |
| Example Color | ![#0a192f](https://via.placeholder.com/10/0a192f?text=+) #0a192f |
| Example Color | ![#f8f8f8](https://via.placeholder.com/10/f8f8f8?text=+) #f8f8f8 |
| Example Color | ![#00b48a](https://via.placeholder.com/10/00b48a?text=+) #00b48a |
| Example Color | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |


## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.

Please adhere to this project's `code of conduct`.


## Demo

Insert gif or link to demo


## Deployment

To deploy this project run

```bash
  npm run deploy
```


## Documentation

[](https://linktodocumentation)

## How to navigate through the code in the jupyter notebook 
### Extraction of Video urls and Video Ids 
1. Open the Jupyter notebook pip install the mentioned libraries.
2. Import the mention libraries.
3. Now create a text file called video_ids 
4. Now execute the first block of code to extract the video urls and video ids for a youtube searchquery that is already given in the code.
5. The output files for this step would be the Djokovic.csv that consists of video urls and the video_ids.txt files which consists of video ids.
### Video Metadata and Comment Data Extraction using the YouTube API with respect to each video id 
1. pip install and import the mentioned libraries.
2. Now execute this block of code with the API mentioned to extract the video metadata and comments data into single csv file called video_metadata.csv
### Classification of Comments as early and steady state responses
1. Import the mentioned libraries.
2. Now execute this block of code that takes video_metadata.csv as input and converts the video, comment timestamps and video duration into seconds and then checks for the core condition if the timestamps difference is less than half of the video duration, if yes it terms that respective comment as early response, else steady state response.
3. The classification of comments is added as a new column called Response_type to the input csv and video_metadata_updated csv is returned.