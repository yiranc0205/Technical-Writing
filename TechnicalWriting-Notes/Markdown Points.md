# Mail Link
Create a mail link that allows the user to send you mail directly**
`[yiranc0205@gmail.com](mailto:yiranc0205@gmail.com)`

Result:
[yiranc0205@gmail.com](mailto:yiranc0205@gmail.com)

# Table of Content
Create a TOC (table of content) within the page**
- Create links to the headings
- Separate spaces in the title with a dash (-)
```
# Table of Contents
1. [Part 1](#Part-1)
2. [Part 2](#Part-2)
```

# Video Reference
Include a YouTube Video Reference**
```html
<!--align left (左对齐)-->
<div align="left">
	<!--link to the video-->
	<a href="https://www.youtube.com/watch?v=Z-vZuBX0Cmk">
		<!--Link to the thumbnail of the video ("Z-vZuBX0Cmk" is the last part of th e video link)-->
		<img src="https://img.youtube.com/vi/Z-vZuBX0Cmk/0.jpg" style="width:100%;">
	</a>
</div>
```

To summarize:
```html
<div align="left">

      <a href="link to my video">

         <img src="https://img.youtube.com/vi/the last part of my link/0.jpg" style="width:100%;">

      </a>

</div>
```