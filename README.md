# Video2mjpeg

This is a (WIP) app for converting videos to the mjpeg format on the Web.

The mjpeg format is simply a concatenation of jpeg images, which are easy to
decode. For this reason, it's used by Video Players for the NumWorks calculator
like:

- [Playa], for [Epsilon], the official firmware (closed-source, based on
  [libjpeg-turbo])
- [Video Player], for [Epsilon], the official firmware (FOSS, based on [Tjpg_Decoder])
- [Video], for [Upsilon], a custom firmware (FOSS, based on [libjpeg-turbo])

Without this app, the recommended way to install apps is to use [ffmpeg], but
people on Windows usually struggle to understand how to launch it. The goal of
this app is to give people an easier way to convert their videos.

## Usage

This section covers how to start the development server and build the app for
production.

### Installing dependencies

Before starting the server, you need to install the dependencies. Just run this
command to get started.

```bash
npm install
```

### Starting the Development Server

To start the development server with hot-reload, run the following command. The
server will be accessible at [http://localhost:3000](http://localhost:3000):

```bash
npm run dev
```

### Building for Production

To build the app for production, use:

```bash
npm run build
```

Once the build process is completed, the application will be ready for
deployment in a production environment.

Files will be stored in the `dist/` folder.

## License

This project is licensed under AGPL 3.0 or later, to allow everyone from freely
using it and preventing people to improve it without helping the community as a
whole.

[Epsilon]: https://github.com/numworks/epsilon
[Upsilon]: https://getupsilon.web.app/

[Playa]: https://yaya-cout.github.io/Nwagyu/guide/apps/playa.html
[Video Player]: https://yaya-cout.github.io/Nwagyu/guide/apps/videoplayer.html
[Video]: https://github.com/UpsilonNumworks/Upsilon-External/tree/master/apps/Video

[libjpeg-turbo]: https://libjpeg-turbo.org/
[Tjpg_Decoder]: https://github.com/Bodmer/TJpg_Decoder
[ffmpeg]: https://ffmpeg.org/
