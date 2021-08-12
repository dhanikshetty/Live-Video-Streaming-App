# Live-Video-Streaming-App
A Simplified Live-Video streaming application developed using React 


## To Run

### Directories

- `client`: The React front-end
- `rtmp`: The Real Time Messaging Protocol (RTMP) Server
- `api`: The API server

In each directory (`client`, `rtmp`, `api`), run `npm install` and then `npm start`. Navigate to `localhost:3000` to begin using the streaming app.

### To stream video

Use streaming software such as [OBS](https://obsproject.com/welcome). Configure your streaming software to stream to the RTMP server. Configuration can be found on [Node-Media-Server](https://github.com/illuspas/Node-Media-Server) for publishing live streams. Configuration should be to the id that you are trying to stream to.


## User Functions
1. Not logged in
    - User can view a list of all stream/channels
    - User can view video for a single stream
2. Logged in
    - User can create a new stream/channel
    - User can **edit** a stream/channel they have created
    - User can **delete** a stream/channel they have created
    
## Tech Stack

- React
- Redux
- React-Router
- JSON Server
- Node-Media-Server

## Information/Data Flow
1. user requests login → googleauthentication →loggged in
2. Streamer’s Computer  records video with  Open Broadcaster Software (OBS) →
    - Video stream + stream key →
3. API - Real Time Messaging Protocol (RTMP) Server →
    - Separate Web Server that knows which streams are currently broadcasting → 
4. Broadcast Video Feed → Multiple Viewers’ Browser →
5. Viewers request to get video from RTMP → viewer…


