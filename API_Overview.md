# APIs: A Brief Overview

API stands for **Application Programming Interface**. APIs provide a way for application developers to request services available across the internet. (We will limit our discussion to Web APIs).

Humans interact with computers through user interfaces. These may be graphical, command-line, or even voice-based. You can think of a developer interacting in a similar way with web-based services, but by using text that can be embedded in web pages or web-based applications.

Most web-based services expose an API. Example services include:

- User authentication
- Weather
- File access
- Ad-serving
- Photos
- Traffic
- Location
- Mapping and route planning
- Search
- Translation

It's safe to say that everything and anything you can do on the web is available through an API.

## API Terminology

### **Endpoint**
The web address of an API's services. Usually resembles a URL.

### **Method**
The feature or function that the developer wishes to call. Endpoints may expose multiple methods.

### **Parameter**
A value provided to the method, and used to calculate a result. A method may accept multiple parameters. Some may be mandatory, some may be optional.

### **Data type**
The required format of a parameter. For example, a parameter that represents a telephone *area code* may be a three-digit integer.

### **Return package**
The value or values returned by the API. May be wrapped in a specialized text format (JSON, XML, HTML).

### **Error Message**
Message returned by an API when it does not recognize or could not process the API call.

### **API Key**
A unique (to the developer or organization) string that authenticates the user of the API. Used to control access to the API, and for tracking API usage for billing purposes.

## Using APIs

The API in our **GetMyWeather** project is fictitious. But there are developer tools for using and testing real APIs. An API similar to our assignment is offered by [OpenWeather](https://openweathermap.org).

[cURL](https://curl.haxx.se) is a popular tool for testing APIs from the command line. cURL comes with MacOS (via the Terminal) and Windows (via the Command Prompt).

You can test the OpenWeather API by running this command. This will get the weather for zip code 15206. The method call also specifies imperial units, and an API key that I have previously registered.

curl --get "https://api.openweathermap.org/data/2.5/weather?zip=15206&units=imperial&appid=33b051b4a84ce79a63d64906ee87230e"








