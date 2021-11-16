# QuoteTool
A tool for glass manufacturing companies to easily build quotes for their customers.

The code itself is currently not available publicly as it belongs to SSAC Consulting. I have however provided some screenshots of the various pages throughout the application to demonstrate each stage of building a quote, viewing saved quotes and exporting quotes to PDF documents.

# Front End
The GUI you see in the screenshots folder was built using JavaFX and Java. It follows the MVC design pattern behind the scenes.

It consists of the following pages/forms: Home, Create Quote Header, Build Quote, Additional Costs, and View Quote.

# Back End
The Back End was built with Java, JDBC and other Java libraries.
The client facing GUI application was set up for two different use cases.

Within company network: The application communicates dirrectly to a relational MSSQL database.

Outside/Within company network: The application communicates to a TCP server hosted within the companies network that processes incoming client requests and handles communication with the database.

The database holds all the normalized data for creating quotes (customer info, product info, pricing, etc) and holds saved quotes for future reference/updates. The client simply communicates to that database with a CRUD request either trough a TCP server or directly.

# Screenshots
![Home1](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/0.%20start1.jpg)
![Home2](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/1.%20start2.jpg)
![Header](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/2.%20header.jpg)
![Triple](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/3.%20triple.jpg)
![Mono](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/4.%20monolithic.jpg)
![Custom](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/5.%20custom.jpg)
![AC](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/6.%20AdditionalCosts.jpg)
![Saved](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/7.%20Saved.jpg)
![ViewQuote](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/8.%20ViewQuote.jpg)
![PDF](https://github.com/Bradyac/QuoteTool/blob/main/Screenshots/9.%20PDF.jpg)
