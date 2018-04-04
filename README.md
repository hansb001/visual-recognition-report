# visual-recognition-report
html code for visual recognition Meetup (report node)


<html>
<head><title>Watson Visual Recognition on Node-RED</title></head>
<body>
<h1>Node-RED Watson Visual Recognition output</h1>
<p>Analyzed image: {{payload}}<br/><img src="{{payload}}" height='100'/></p>
<table border='1'>
    <thead><tr><th>Name</th><th>Score</th></tr></thead>
{{#result.images.0.classifiers.0.classes}}
  <tr><td><b>{{class}}</b></td><td><i>{{score}}</i></td></tr>
{{/result.images.0.classifiers.0.classes}}
</table>
<form  action="{{req._parsedUrl.pathname}}">
    <input type="submit" value="Try again"/>
</form>
</body>
</html>



# Fac647d7b10ef2cea125910b11ec0538bf37df07


# 3ed1f1e8ee680df62faf3ed5a4e6eb4d19faebd6
