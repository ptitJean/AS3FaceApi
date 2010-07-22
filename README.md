AS3 port of the face.com API

Need as3crypto.swc if you want use OAuth( for Twitter auth ).


### Usage ###

	var faceApi:FaceApi = new FaceApi();
	faceApi.apiKey = "your_api_key";
	faceApi.apiSecret = "your_api_secret";

	faceApi.recognitionService.recognize( urls , uids );
	faceApi.recognitionService.addEventListener( FaceEvent.SUCCESS , recoHandler );

	function recoHandler( evt : FaceEvent ) : void
	{
		var result:Object = evt.data;
	}