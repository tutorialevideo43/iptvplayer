# iptvplayer
simple iptv video player
m3u8 url 
 hls.loadSource('example.m3u8');
    hls.attachMedia(video);
    video.play();
  }
  else if (video.canPlayType('application/vnd.apple.mpegurl')) {
    video.src = 'example.m3u8';
    video.addEventListener('loadedmetadata',function() {
      video.play();
    });
  }
 
