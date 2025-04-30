# Global Social Media Analytics Platform
![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter%20Notebook-%E2%9C%94-F37626?logo=jupyter&logoColor=white)
![Git](https://img.shields.io/badge/Git-2.49.0-f05133?logo=git&logoColor=white)
![Twitter API](https://img.shields.io/badge/Twitter_API-565656.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAACXBIWXMAAAsTAAALEwEAmpwYAAACwElEQVR4nO2YT4hPURTHr3PmmYU/oSQWdiLlX5KFUogyIvmz8Cf5t8SGrGQWiixFGqWI/Oac22gkZkWyU6SRKAsiJZphfr93zhsy+T2950emZqb3e/e9N5v3qbt7797zPefce889xpSUlJSUlJQkxNbmI+kFZH2NJAGy1oDlObKcMbd19ki/eBVZbFzATt1o2kNwmqQ9hMhIJBlC1nDEQSpAejj+/k7fFCR/O7A+QtKL6Re2XyYjaTXymov9SHJlVMN5+ACSZ8jy848o+WRsdYbDwtr2n4cuGxtis3OAld1JjcfhEen3rC41t6rTsVPWpRIAVo4M8w7L3aY8EoYTkORt88bLELB2AetjJP3qWVmUTgDLsREm/4hW1if5v4WCFam8z3+HfEcbbDFpQQo2j5qrLN2my18wpgNIDzgI6Gshf5VxIj4NVMYIdR1I7kVCTU/YmiiCSTczyy6TBY1zO8mitUbenkAra01XbR6w7E0dgU5/WyYCzI1wErK+ccvlNAJ0g7PtQLIHSPd5FV0GLL1FCvDSnjyj5jDJYGECSOpR5J0FRBdJ4anD8SX2ymQFsDwpXoR0ZCbAs8Hyf7VJcRFoM1mCJDsLE0Hab2w40WRNVBYAy9P8Bcg5kwdIwVa0uglJriHJj5yMHzSVYE5OAvRSAZv3vMkN689E1s85ps4Hc7N/an4Con1QCVYi67ccPP8raYnuTlSkkT7MUgBYPW2KJrofgLQdWB84ps716OVWuIBoUWA9iKQDTsbb5t/ZbvSErWB1P7C+cDC8DqSncvW8R7okSpMW8lej9XcA6UlguY+kvmPKvEOSNSZ3ugemIcvZRgctg2NSq7HXsyiTm6Iis4DkOLC+THXCsPQCydHIIWbcsf5CsHoISa7GZXbU84k7d1KP7weS93E7kKUjbhPawbnjbXJJSUlJSUmJyZHfxnHsrRJKPnUAAAAASUVORK5CYII=)

This project analyzes global user engagement patterns by focusing on Greta Thunberg's Twitter followers, leveraging data from the Twitter API and Python for data processing and analysis.

## Features
- Developed a data analytics pipeline to collect and process Twitter user data from two countries.
- Analyzed geographic distribution, user biographies, and posting behavior of followers.
- Identified socio-cultural and geographic trends within follower groups, uncovering regional engagement styles and community structures.

## Architecture
<div>
<table>
  <tr>
    <td >
<pre>
                  Batch Processing
                +---------------------+
                |   Twitter API       |
                +---------------------+
                         |
                         v
                +---------------------+
                |  Data Collection    |
                +---------------------+
                         |
                         v
                +---------------------+
                |  Raw Data Storage   |
                +---------------------+
                         |
                         v
                +---------------------+
                | Data Processing &   |   now                next
                | Preprocessing       |   ------------------------->
                +---------------------+
                         |
                         v
                +---------------------+
                | Exploratory Data    |
                | Analysis (EDA)      |
                +---------------------+
                         |
                         v
                +---------------------+
                | Trend Detection &   |
                | Insights Extraction |
                +---------------------+
                         |
                         v
                +---------------------+
                |   Visualization &   |
                |   Reporting         |
                +---------------------+
</pre>
    </td>
    <td >
<pre>
                  Real Time Processing
                +-----------------------+
                | Twitter Streaming API |
                +-----------------------+
                            |
                            v
            +------------------------------+
            |  Stream Processor (Python)   |
            |   (Tweepy StreamListener)    |
            +------------------------------+
                            |
                            v
        +-------------------------------------------+
        |  Message Broker (Apache Kafka / RabbitMQ) |
        +-------------------------------------------+
                            |
                            v
        +-------------------------------------------+
        |     Stream Consumer & Data Processor      |
        |         (Python + Pandas/Numpy)           |
        +-------------------------------------------+
                            |
                            v
        +-----------------------------------------+
        |           Real-time Storage             |
        | (ElasticSearch / MongoDB / TimescaleDB) |
        +-----------------------------------------+
                            |
                            v
        +------------------------------------------+
        |          Real-Time Dashboards            |
        | (Kibana / Grafana / Custom Python Dash)  |
        +------------------------------------------+
</pre>
    </td>
  </tr>
</table>
</div>



## Business Impact
- Provided data-driven insights to help influencers and organizations enhance social media strategies and engagement in digital activism.
- Supported Corporate Social Responsibility (CSR) campaigns by identifying key demographic groups and engagement trends.
