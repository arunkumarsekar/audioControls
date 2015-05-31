# audioControls
Simple way to create your own audio player.

## Features
- playlist
- audio repeat
- shuffle playlist
- repeat audio
- repeat playlist
- audio timer (increment / decrement)
- seekable track
- buffer loader & default player controls
- easy to integrate
- suitable for maximum theme
- Api's and documentation

## Requirements
- jQuery
- HTML5

## Example
Here is basic example of using audioControls.
Design your own theme how ever you want and just pust *data-attr* appropriate places.

### HTML
```HTML
<div class="twoColumn">
	<!-- Audio Player Control's -->
	<div class="col-1 toolsPane">
		<a href="#" title="Show/Hide Playlist" alt="Show/Hide Playlist"><span class="ctrls playlist"></span></a>
		<a href="#" title="Previous Song" alt="Previous Song"><span data-attr="prevAudio" class="ctrls previous"></span></a>
		<a href="#" title="Play/Pause" alt="Play/Pause"><span data-attr="playPauseAudio" class="ctrls playAudio"></span></a>
		<a href="#" title="Next Song" alt="Next Song"><span data-attr="nextAudio" class="ctrls next"></span></a>
		<a href="#" title="Repeat Song" alt="Repeat Song"><span data-attr="repeatSong" class="ctrls replay"></span></a>
	</div>
	<div class="volumeControlContainer">
		<input data-attr="rangeVolume" type="range" min="0" max="1" step="0.1" />
	</div>
	<!-- EOF Audio Player Control's -->
	<!-- Playlist -->
	<div id="audioPlayer" class="col-2 container">
		<div class="playlistContainer">
			<ul id="playlist">
				<li data-src="songs/Everything But Mine.mp3">
					<a href="#">
						<img src="images/thumbs/bsb.jpg" />
						BSB - Everything But Mine
					</a>
				</li>
				<li data-src="songs/Linkin Park - Numb.mp3">
					<a href="#">
						<img src="images/thumbs/linkin-park.jpg" />
						Linkin Park - Numb
					</a>
				</li>
				<li data-src="songs/love-the-way-you-lie-rihanna-feat-eminem.mp3">
					<a href="#">
						<img src="images/thumbs/eminem.jpg" />
						Eminem - Love The Way You Lie(Rihanna Ft)
					</a>
				</li>
				<li data-src="songs/rolling-in-the-deep-adele.mp3">
					<a href="#">
						<img src="images/thumbs/adele.jpg" />
						Adele - Rolling In The Deep
					</a>
				</li>
				<li data-src="songs/when-i-was-your-man-bruno-mars.mp3">
					<a href="#">
						<img src="images/thumbs/bruno-mars.jpg" />
						Bruno - When I Was Your Man
					</a>
				</li>
			</ul>
		</div>
	</div>
	<!-- EOF Playlist -->
</div>
```
### Note
Removed songs folder and mp3's, add songs folder to keep demo working

### jQuery
```javascript
$(document).ready(function(){
	$("#audioPlayer").audioControls();
});
```
## License
This plugin available under [MIT license](http://opensource.org/licenses/mit-license.php)

