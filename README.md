# SVG-To-TXT
A short python snippet that converts SVG to PNG and then converts it to TXT using [Google Cloud Vision API](https://cloud.google.com/vision/docs/ocr#vision_text_detection_gcs-python) 

In order to use this code, Sign up [here](https://console.cloud.google.com/freetrial/signup/tos?_ga=2.93536797.1081095021.1670258729-705070752.1664365819&facet_utm_source=google&facet_utm_campaign=(organic)&facet_utm_medium=organic&facet_url=https:%2F%2Fcloud.google.com%2Fvision%2Fdocs%2Focr&facet_id_list=%5B39300012,%2039300020,%2039300118,%2039300195,%2039300251,%2039300319,%2039300320,%2039300325,%2039300333,%2039300346,%2039300354,%2039300364,%2039300373,%2039300408,%2039300421,%2039300437%5D)
in google cloud and get a key.json from cloud console. 

### Steps Followed:

1. Python ['svglib'](https://pypi.org/project/svglib/) is used to convert the SVG file into *ReportLab Graphics Drawing objects*.
2. The *ReportLab Graphics Drawing object* is converted to PNG using the [reportlab](https://docs.reportlab.com/) library.
3. Generated "*.png*" file is passed to google cloud api and converted into TXT.
