<h1 align="center">Hey, I'm <a href="https://katuha1.github.io/web-site/" target="_blank">Katuha</a> 
<img src="https://kittyclub.ru/wp-content/uploads/2015/08/cat-vampire-e1440582745634.jpg" height="32"/></h1>
<h3>I'm in college and 18 years old.</h3>

<div>
<img height="180em" src="https://github-readme-stats.vercel.app/api?username=katuha1&show_icons=true&include_all_commits=true&count_private=true"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=katuha1&layout=compact&langs_count=6"/>
</div>

<body onload="countdown()">
	<div id="days"></div>
	<p id="happy_new_year"></p>
</body>

<script>
	function countdown() {
		let _second = 1000;
		let _minute = _second * 60;
		let _hour = _minute * 60;
		let _day = _hour * 24;
        let distance = new Date('01/01/2023 12:00 PM') - new Date();;
		
		let days = Math.floor(distance / _day);
        let hours = Math.floor((distance % _day) / _hour);
        let minutes = Math.floor((distance % _hour) / _minute);
        let seconds = Math.floor((distance % _minute) / _second);
		
		document.getElementById('days').innerHTML = days + ' Days';
		document.getElementById('happy_new_year').innerHTML = hours + ":" + minutes + ":" + seconds;
		setTimeout("countdown()", 1000);
	}
</script>
