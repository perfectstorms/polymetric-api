# polymetric-server

[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://mit-license.org/)
[![JDK](https://img.shields.io/badge/JDK-%3E%3D%201.8-d36e6e.svg?style=flat-circle)](https://docs.oracle.com/javase/8/docs/)
<br>

## Task
Create a Spring Boot REST API Service for the <a href="https://github.com/perfectstorms/polymetric-client">polymetric-client</a>.

## Technologies
Java 8<br>
Spring Boot 2.1.5<br>
Spring Data<br>
Hibernate<br>
Postgresql<br>
Lombok<br>
Devtools<br>
Maven<br>

## How to run the application?
Package the project with using maven fo create jar file:
```
mvn package
```

Run application:
```
jar tvf target/polymetrica-0.0.1-dev.jar
java -jar target/polymetrica-0.0.1-dev.jar
```

after open your  browser: <a href="http://127.0.0.1:8080/actions/video">127.0.0.1:8080/actions/video</a>

<img src="https://i.ibb.co/PgLv9ZS/video.png">


## API
We provide a REST service for easy management with data from the database.

#### Video actions
| Type | Path | Description | Parameters |
| --- | --- | --- | --- |
| GET | `/actions/video/` | List all video actions | &mdash; |
| GET | `/actions/video/{id}` | Get one video action by {id} | id:long |
| POST | `/actions/video/add` | Add new video action | username (String)<br>type_id (long)<br>time (HH:MM:SS)<br>date: (YY-MM-DD)<br>videoId (long)<br>videoPosition (HH:MM:SS)<br>rePosition (HH:MM:SS) |

#### Video action types
| Type | Path | Description | Parameters |
| --- | --- | --- | --- |
| GET | `/actions/video/types` | List all video action types | &mdash; |
| GET | `/actions/video/types/{id}` | Get one video action typeId by {id} | id:long |

## Contribute
For any problems, comments, or feedback please create an issue [here on GitHub](https://github.com/perfectstorms/polymetric-client/issues).
<br>

## Licence
Game of Life is released under the [MIT license](https://en.wikipedia.org/wiki/MIT_License).