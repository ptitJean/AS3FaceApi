AS3 port of the face.com API

Need as3crypto.swc & Crypto.swc( it will be soon go on one of them ).


### Usage ###

	var faceApi:FaceApi = new FaceApi();
	faceApi.apiKey = "dbcfca68572671b4c26a43d7231df505";
	faceApi.apiSecret = "34ddf640f49747318df77a0d71e79ae3";

	faceApi.recognitionService.recognize( urls , uids );
	faceApi.recognitionService.addEventListener( FaceEvent.SUCCESS , recoHandler );

	function recoHandler( evt : FaceEvent ) : void
	{
		var result:Object = evt.data;
	}