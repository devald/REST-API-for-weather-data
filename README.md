# Weather REST API
## Prerequisite
API key for [OpenWeatherMap](https://openweathermap.org/current) and [Weather Underground](https://www.wunderground.com/weather/api/d/docs).
## Usage
First, you need to set the right environment variables.

`set -gx OWM_API_KEY <your OpenWeatherMap API key>`

and

`set -gx WU_API_KEY <your Weather Underground API key>`
## Run
`go run main.go`
## Test
`curl -s http://localhost:8080/weather/<name of the city>`

For example:

`curl -s http://localhost:8080/weather/dachau`

Result:

`{"city":"dachau","temp":3.85,"took":"332.12037ms"}`
