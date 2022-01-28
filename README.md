# node-red-number-plate-recognition
Thir epository will have my flos for number plate recognition

register for free 2000 requests from web here https://app.platerecognizer.com/<br>
Get Token and update node with your token

## Here is test code to see if your token work

    curl -o /tmp/car.jpg https://app.platerecognizer.com/static/demo.jpg # Get an image
    curl -F "upload=@/tmp/car.jpg" -F regions=us-ca \
    -H "Authorization: Token yout token here" \
    https://api.platerecognizer.com/v1/plate-reader
