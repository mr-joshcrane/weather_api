### Example import:
 ```go
import "github.com/mr-joshcrane/weather_api"
```

### Example of Library Usage
 ```go
conditions, err := weather_api.Get(location, API_KEY)
if err != nil {
    //handle error appropriately
}
fmt.Println(conditions)
```

### Example of CLI usage (bash)
 ```bash
go build -o weather src/main.go
./weather Perth,AU
```

### What is it and why would I use it?

A simple, easy to use library that creates a client that leverages the OpenWeatherMap API (https://openweathermap.org/api). If you want basic weather information about a location, this might do the job for you!

### OpenWeatherMap API Key
To use the OpenWeatherMap API, you need an API Key, see instructions at their FAQ on how to obtain one (https://openweathermap.org/faq).

Once you have the key, you should set it as the OPENWEATHERMAP_API_KEY environment variable.

Mac/Unix
```bash
export OPENWEATHERMAP_API_KEY=yourAPIKeyhere 
```

Windows
```command line
set OPENWEATHERMAP_API_KEY=yourAPIKeyhere
```
