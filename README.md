
**WELCOME TO MY GITHUB PROFILE!**
- 👋 Hi, I’m @Proxypro2012
- 👀 I’m interested in ... anything techonology related
- 🌱 I’m currently learning ... python and scratch. Working on getting my app (RollMate) out into schools.
- 💞️ I’m looking to collaborate on ... nothing at the moment. But mostly scratch games.
- 📫 How to reach me ... my username on scratch is @-Refracted- . Message me there.
- 😄 Pronouns: ... He/Him
- ⚡ Fun fact: ... I am 12 years old and am in 7th grade.

<img align="left" src="https://github-readme-stats.vercel.app/api?username=Proxypro2012&include_all_commits=true&count_private=true&show_icons=true&line_height=20&title_color=2B5BBD&icon_color=1124BB&text_color=A1A1A1&bg_color=0,000000,130F40" alt="my Github Stats"/>


<img align="right" src="https://github-readme-streak-stats.herokuapp.com/?user=Proxypro2012&theme=tokyonight" alt="mystreak"/>


/*
*
* Simple Parallax, 01/03/2012
*
* Contributors
* @felquis, @cironunesdev
* DEMO: http://jsfiddle.net/6qhVN/
*/

!(function( $, window, document ) {
    var $doc = $(document),
            body = document.body,
            val = 0.2,
            limit = 1;

    $(function(){

      $doc.on('mousemove', function( e ){

            var //first proprities to calculate the parallax
            xMouse = e.pageX,
            yMouse = e.pageY,
            xCenter = body.clientWidth / 2,
            yCenter = body.clientHeight / 2,
            offsetLeft = xMouse - xCenter,
            offsetTop = yMouse - yCenter,
            i,

            //then caching dom elem and your lenght
            $elem = $('.parallax-item');

            $elem.each(function( i ) {
                $(this).css({
                    left: offsetLeft * val,
                    top: offsetTop * val
                });

                console.log(val);

                val += 0.2;

                if( val === limit ) {
                    val = 0.2;
                }
            });

        });

    });
}( jQuery, window, document ))




