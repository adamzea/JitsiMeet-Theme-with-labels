# JitsiMeet-Theme-with-labels
Jitsi Meet CSS code that improves usability by labeling navigation buttons

Edit the body.html file using: 
sudo nano /usr/share/jitsi-meet/body.html

Add the CSS code to enable the theme:
```sh
<style>
.welcome .header {
    background-image: linear-gradient(0deg,rgba(255,255,255,.2),rgba(255,255,255,.8)),url(https://www.rohersprague.com/images/90NBroadway_DSC3540.jpg);
    background-position: center;
    background-repeat: none;
    background-size: cover;
    padding-bottom: 55px;
    background-color: #131519;
    overflow: hidden;
    position: relative;
}

.welcome .header .header-text-title { display: none; }
.welcome .header .header-text-subtitle {display: none; }
.watermark.leftwatermarknomargin {
    background-image: url(https://www.rohersprague.com/images/RS-LOGObw2.svg)!important;
max-width: 300px!important;
max-height:100px!important;
width: 150px!important;
height: 60px!important;
position: static; }

.watermark { width: 150px!important;
height: 60px!important; }

.welcome .header #enter_room {
        margin-top: 100px;
        margin-bottom: 100px;
}

.welcome .welcome-page-settings {
    background: rgba(0,0,0,.38);
    border-radius: 3px;
    color: #fff;
}

/* add labels to toolbar */
.toolbox-button {
width: 7vw;}

.toolbox-button:after {
content: attr(aria-label); font-size: 0.7rem;
line-height: 0.8rem;
}

.toolbox-icon {
width: 100%; }

.welcome-page-settings .toolbox-button {
display: flex;}

.reactions-row .toolbox-button { width: 30%; }
.reactions-row .toolbox-icon span.emoji { width: 5rem; }
.reactions-row .toolbox-icon { width: 5rem; }

/* mobile stuff */
@media only screen and (max-width: 500px) {
.welcome .header #enter_room {
```
    width: 95%!important;

}
}
</style>

