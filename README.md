# Test Server

`npm run tserver`

# API documentation

## `GET /api/events` Response:

```js
[
  {
    date: "yyyy-mm-ddT00:00:00.000Z",
    description: string,
    id: string(20),
    location: string,
    max_team_size: int,
    min_team_size: int,
    name: string,
    participants: int,
    photos: [ string(20)... ],
    registration_start: "yyyy-mm-ddT00:00:00.000Z",
    synopsis: string,
  },...
]
```

## `GET /api/events/string(20)`

```js
{
  date: "yyyy-mm-ddT00:00:00.000Z",
  description: string,
  id: string(20),
  location: string,
  max_team_size: int,
  min_team_size: int,
  name: string,
  participants: int,
  photos: [ string(20)... ],
  registration_start: "yyyy-mm-ddT00:00:00.000Z",
  synopsis: string,
}
```

## `GET /images/are/not/here/string(20)` -> image

## `GET /api/podcasts`

```js
[
  {
    description: string,
    guests: [ string... ],
    id: string(20),
    image: string(20),
    mime: string,
    name: string,
    publish: bool,
  },...
]
```

## `GET /api/podcasts/string(20)`

```js
{
  description: string,
  guests: [ string... ],
  id: string(20),
  image: string(20),
  mime: string,
  name: string,
  publish: bool,
}
```

## `GET /api/podcast/string(20)/stream` -> audio

## `GET /api/credits`

```js
[
  {
    name: string,
    contributions: string,
  },...
]
```

## `GET /api/members`

```js
[
  {
    description: string,
    dimension: string,
    energy: string,
    features: string,
    hobbies: string,
    id: string(20),
    name: string,
    photos: [ string(20)... ],
    portfolio: string,
    role: string,
    type: string,
  },...
]
```

## `GET /api/members/string(20)`

```js
{
  description: string,
  dimension: string,
  energy: string,
  features: string,
  hobbies: string,
  id: string(20),
  name: string,
  photos: [ string(20)... ],
  portfolio: string,
  role: string,
  type: string,
}
```

<!-- ## `GET /api/captcha`

```js
{
  captcha: string,
  token: string,
}
``` -->
