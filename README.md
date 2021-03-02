# Gulp template
<h3>
File 'gulpfile.js' views files from '#src' folder and builds them in 'name of project_dir' folder. You can use it to simplify the work on the front-end part of web-app.
</h3>
<h3>Here's a description of what exactly the gulp does:</h3>
<ul>
	<li style="font-size: 18px"> <b>html</b>: copies all html files, which do not start with '_'. Before copying it replaces all @@include('_*.html') strings with the code in corresponding partial representations (which should start with '_'); change all <img> tags to 'picture + source + img' combination.
	</li>
	<li style="font-size: 18px"> <b>css</b>: compile all 'scss' files to css and min.css, grouping by media.
	</li>
	<li style="font-size: 18px"> <b>js</b>: copy all 'js' files to js and min.js.
	</li>
	<li style="font-size: 18px"> <b>images</b>: copy image from the source folder and create copy with 'wepb'.(thats why we convert img to picture combination in html).
	</li>
	<li style="font-size: 18px"> <b>fonts</b>:  convert otf to ttf if (using specified gulp task),
	then make 'woff'/'woff2' fonts and write them in css.
	</li>
</ul>
<h3> Also by default runs "watch" witch watches all the changes in #src and change destination folder automatically.</h3>
Don't forget to run "npm i" to install all node_modules from 'package.json'.
