# Timestamp Microservice

This Timestamp Microservice, implemented using Node.js and Express.js, allows users to retrieve the current Unix timestamp and UTC time or convert a given date string or Unix timestamp to Unix timestamp and UTC time.

## Usage Example

### Get Current Unix Timestamp and UTC Time

- **Endpoint**: GET `/api/`
- **Response**:

  ```json
  {
    "unix": 1643988253073,
    "utc": "Sat, 05 Feb 2022 10:30:53 GMT"
  }
  ```

### Convert Date String or Unix Timestamp

- **Endpoint**: GET `/api/:date`
- **Parameters**:
  - `:date`: A valid date string or Unix timestamp.
- **Response**:

  ```json
  {
    "unix": 1643988253073,
    "utc": "Sat, 05 Feb 2022 10:30:53 GMT"
  }
  ```

  If the input date string is invalid:

  ```json
  {
    "error": "Invalid Date"
  }
  ```
