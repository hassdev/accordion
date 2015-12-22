<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8" />
<link rel="stylesheet" href="reset.css" />
<title>accordion test</title>

<style>
	html,body { font-size: 14px }
	dl {
		border: solid 1px #ccc;
		padding: 1em;
	}
	dt {
		border: solid 1px #ffbfec;
		padding: 1em;
		font-weight: bold;
		/* Permalink - use to edit and share this gradient: http://colorzilla.com/gradient-editor/#fff2fc+0,ffddf6+100 */
		background: #fff2fc; /* Old browsers */
		background: -moz-linear-gradient(top,  #fff2fc 0%, #ffddf6 100%); /* FF3.6-15 */
		background: -webkit-linear-gradient(top,  #fff2fc 0%,#ffddf6 100%); /* Chrome10-25,Safari5.1-6 */
		background: linear-gradient(to bottom,  #fff2fc 0%,#ffddf6 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
		filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#fff2fc', endColorstr='#ffddf6',GradientType=0 ); /* IE6-9 */
	}
	dd {
		border: solid 1px #b7cdff;
		padding: 1em;
		/* Permalink - use to edit and share this gradient: http://colorzilla.com/gradient-editor/#f2f7ff+0,dde7ff+100 */
		background: #f2f7ff; /* Old browsers */
		background: -moz-linear-gradient(top,  #f2f7ff 0%, #dde7ff 100%); /* FF3.6-15 */
		background: -webkit-linear-gradient(top,  #f2f7ff 0%,#dde7ff 100%); /* Chrome10-25,Safari5.1-6 */
		background: linear-gradient(to bottom,  #f2f7ff 0%,#dde7ff 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
		filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f2f7ff', endColorstr='#dde7ff',GradientType=0 ); /* IE6-9 */
	}
</style>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
<script>
	$(function() {
		$("dd").hide();
		$("dt").click(function() {
			var dd_p = $(this).parent();
			var dd = $(this).next();
			dd.slideToggle(150);
			dd_p.find("dd").not(dd).slideUp(150);
		});
	});
</script>
</head>

<body>
	<dl>
		<dt>Definition Term 1</dt>
		<dd>Definition Description 1</dd>

		<dt>Definition Term 2</dt>
		<dd>Definition Description 2</dd>

		<dt>Definition Term 3</dt>
		<dd>Definition Description 3</dd>

		<dt>Definition Term 4</dt>
		<dd>Definition Description 4</dd>
	</dl>

	<dl>
		<dt>Definition Term 1</dt>
		<dd>Definition Description 1</dd>

		<dt>Definition Term 2</dt>
		<dd>Definition Description 2</dd>

		<dt>Definition Term 3</dt>
		<dd>Definition Description 3</dd>

		<dt>Definition Term 4</dt>
		<dd>Definition Description 4</dd>
	</dl>

	<dl>
		<dt>Definition Term 1</dt>
		<dd>Definition Description 1</dd>

		<dt>Definition Term 2</dt>
		<dd>Definition Description 2</dd>

		<dt>Definition Term 3</dt>
		<dd>Definition Description 3</dd>

		<dt>Definition Term 4</dt>
		<dd>Definition Description 4</dd>
	</dl>
</body>
</html>
