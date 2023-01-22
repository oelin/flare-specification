# Flare Specification 1.0.0

## 1. Playlists

### 1.1. Syntax

A Flare playlist MUST be a *valid*, UTF-8 encoded YAML file with the following structure:

```yaml
<Stream 0 Name>:
    headers:
        ...
    content:
        - <Chunk 0 URL>
        - <Chunk 1 URL>
        - ...

<Stream 1 Name>:
    headers:
        ...
    content:
        - <Chunk 0 URL>
        - <Chunk 1 URL>
        - ...
```

where:

* Stream names MUST be unique.
* Chunk URLs SHOULD be unique.
* Chunk URLs MUST use HTTP or HTTPS.


### 1.2. Semantics

Stream headers SHOULD be interpreted by the client.
