---document.querySelector("#myButton").addEventListener("click", async () => {
  if (!navigator.mediaDevices.selectAudioOutput) {
    console.log("selectAudioOutput() not supported or not in secure context.");
    return;
  }

  // Display prompt to select device
  const audioDevice = await navigator.mediaDevices.selectAudioOutput();

  // Create an audio element and start playing audio on the default device
  const audio = document.createElement("audio");
  audio.src = "https://example.com/audio.mp3";
  audio.play();

  // Change the sink to the selected audio output device.
  audio.setSinkId(audioDevice.deviceId);
});
https://www.shah-nar.az/haqqimizda/{"constant":false,"inputs":[],"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"constant":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"address","name":"approved","type":"address"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"Approval","payable":false,"type":"event"},{"constant":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"address","name":"operator","type":"address"},{"indexed":false,"internalType":"bool","name":"approved","type":"bool"}],"name":"ApprovalForAll","payable":false,"type":"event"},{"constant":false,"inputs":[{"indexed":true,"internalType":"address","name":"previousOwner","type":"address"},{"indexed":true,"internalType":"address","name":"newOwner","type":"address"}],"name":"OwnershipTransferred","payable":false,"type":"event"},{"constant":false,"inputs":[{"indexed":true,"internalType":"address","name":"from","type":"address"},{"indexed":true,"internalType":"address","name":"to","type":"address"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"Transfer","payable":false,"type":"event"},{"constant":false,"inputs":[],"name":"MAX_PUBLIC_MINT","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"MAX_SUPPLY","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"PRICE_PER_TOKEN","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"PROVENANCE","outputs":[{"internalType":"string","name":"","type":"string"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"to","type":"address"},{"indexed":false,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"approve","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"owner","type":"address"}],"name":"balanceOf","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"getApproved","outputs":[{"internalType":"address","name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"isAllowListActive","outputs":[{"internalType":"bool","name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"owner","type":"address"},{"indexed":false,"internalType":"address","name":"operator","type":"address"}],"name":"isApprovedForAll","outputs":[{"internalType":"bool","name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"numberOfTokens","type":"uint256"}],"name":"mint","outputs":[],"payable":false,"stateMutability":"payable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"uint8","name":"numberOfTokens","type":"uint8"}],"name":"mintAllowList","outputs":[],"payable":false,"stateMutability":"payable","type":"function"},{"constant":false,"inputs":[],"name":"name","outputs":[{"internalType":"string","name":"","type":"string"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"addr","type":"address"}],"name":"numAvailableToMint","outputs":[{"internalType":"uint8","name":"","type":"uint8"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"owner","outputs":[{"internalType":"address","name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"ownerOf","outputs":[{"internalType":"address","name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"renounceOwnership","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"n","type":"uint256"}],"name":"reserve","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"from","type":"address"},{"indexed":false,"internalType":"address","name":"to","type":"address"},{"indexed":false,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"safeTransferFrom","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"from","type":"address"},{"indexed":false,"internalType":"address","name":"to","type":"address"},{"indexed":false,"internalType":"uint256","name":"tokenId","type":"uint256"},{"indexed":false,"internalType":"bytes","name":"_data","type":"bytes"}],"name":"safeTransferFrom","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[],"name":"saleIsActive","outputs":[{"internalType":"bool","name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address[]","name":"addresses","type":"address[]"},{"indexed":false,"internalType":"uint8","name":"numAllowedToMint","type":"uint8"}],"name":"setAllowList","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"operator","type":"address"},{"indexed":false,"internalType":"bool","name":"approved","type":"bool"}],"name":"setApprovalForAll","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"string","name":"baseURI_","type":"string"}],"name":"setBaseURI","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"bool","name":"_isAllowListActive","type":"bool"}],"name":"setIsAllowListActive","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"string","name":"provenance","type":"string"}],"name":"setProvenance","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"bool","name":"newState","type":"bool"}],"name":"setSaleState","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"bytes4","name":"interfaceId","type":"bytes4"}],"name":"supportsInterface","outputs":[{"internalType":"bool","name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"symbol","outputs":[{"internalType":"string","name":"","type":"string"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"index","type":"uint256"}],"name":"tokenByIndex","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"owner","type":"address"},{"indexed":false,"internalType":"uint256","name":"index","type":"uint256"}],"name":"tokenOfOwnerByIndex","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"tokenURI","outputs":[{"internalType":"string","name":"","type":"string"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"totalSupply","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"from","type":"address"},{"indexed":false,"internalType":"address","name":"to","type":"address"},{"indexed":false,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"transferFrom","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"indexed":false,"internalType":"address","name":"newOwner","type":"address"}],"name":"transferOwnership","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[],"name":"withdraw","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"}]package mediawiki

import (
	"fmt"
	"io/ioutil"
	"net/http"
	"net/http/httptest"
	"net/url"
	"strings"
	"testing"
)

const (
	editTokenReponse = `{"query":{"pages":{"15580374":{"pageid":15580374,"ns":0,"title":"Main Page","contentmodel":"wikitext","pagelanguage":"en","touched":"2013-11-02T14:08:05Z","lastrevid":574690625,"counter":"","length":6391,"starttimestamp":"2013-11-02T15:24:43Z","edittoken":"+\\","revisions":[{"revid":574690625,"parentid":574690493,"minor":"","user":"Tariqabjotu","timestamp":"2013-09-27T03:10:17Z","comment":"removing unnecessary pipe"}]}}}}`
	firstLogin       = `{"login":{"result":"NeedToken","token":"8f48670ddc7fa9d5fa7e7fa2ae147e80","cookieprefix":"wikidb","sessionid":"927e0d298f6f3b5bb21228803fd9c0eb"}}`
	secondLogin      = `{"login":{"result":"Success","token":"8f48670ddc7fa9d5fa7e7fa2ae147e80","cookieprefix":"wikidb","sessionid":"927e0d298f6f3b5bb21228803fd9c0eb"}}`
	failedLogin      = `{"login":{"result":"ERROR THING","token":"8f48670ddc7fa9d5fa7e7fa2ae147e80","cookieprefix":"wikidb","sessionid":"927e0d298f6f3b5bb21228803fd9c0eb"}}`
	readPage         = `{"query-continue":{"revisions":{"rvcontinue":574690493}},"query":{"pages":{"15580374":{"pageid":15580374,"ns":0,"title":"Main Page","revisions":[{"user":"Tariqabjotu","timestamp":"2013-09-27T03:10:17Z","comment":"removing unnecessary pipe","contentformat":"text/x-wiki","contentmodel":"wikitext","*":"FULL PAGE TEXT"}]}}}}`
	fileURL          = `{"query":{"pages":{"107":{"pageid":107,"ns":6,"title":"File:stuff.pdf","imagerepository":"local","imageinfo":[{"url":"%s","descriptionurl":"TEST"}]}}}}`
	fileURLFailed    = `{"query":{"pages":{"544100":{"pageid":544100,"ns":0,"title":"Asdf"}}}}`
	mwerror          = `{"servedby":"mw1123","error":{"code":"unknown_action","info":"Unrecognized value for parameter 'action': blah"}}`
	editsuccess      = `{"Edit":{"result":"Success","pageid":12,"title":"Talk:Main Page","oldrevid":465,"newrevid":471}}`
	editfailure      = `{"Edit":{"result":"Failure!","pageid":12,"title":"Talk:Main Page","oldrevid":465,"newrevid":471}}`
)

type Test struct {
	ts     *httptest.Server
	client *MWApi
}

func (t *Test) TearDown() {
	t.ts.Close()
}

func BuildUp(response string, t *testing.T) *Test {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		fmt.Fprintln(w, response)
	}))
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error in BuildUp: %s", err)
	}
	return &Test{ts: ts, client: client}
}

func TestGetEditToken(t *testing.T) {
	test := BuildUp(editTokenReponse, t)
	defer test.TearDown()

	err := test.client.GetEditToken()
	if err != nil {
		t.Errorf("Could not get edit token: %s", err.Error())
	} else {
		t.Log("Got edit token")
	}
	if test.client.edittoken == `+\` {
		t.Log("Edit token correct")
	} else {
		t.Errorf("Incorrect edit token: %s", test.client.edittoken)
	}
}

func TestLogin(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		err := r.ParseForm()
		if err != nil {
			panic(err)
		}
		if r.Form.Get("lgtoken") == "" {
			fmt.Fprintln(w, firstLogin)
		} else {
			fmt.Fprintln(w, secondLogin)
		}
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err.Error())
	}
	client.Domain = "asdf"
	err = client.Login("asdf", "asdf")
	if err != nil {
		t.Errorf("Client failed to login: %s", err)
	} else {
		t.Log("Client logged in successfully.")
	}
}

func TestLoginFailedSecondary(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		err := r.ParseForm()
		if err != nil {
			panic(err)
		}
		if r.Form.Get("lgtoken") == "" {
			fmt.Fprintln(w, firstLogin)
		} else {
			fmt.Fprintln(w, failedLogin)
		}
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err)
	}
	client.Domain = "asdf"
	err = client.Login("asdf", "asdf")
	if err == nil {
		t.Error("Client logged in successfully. (BUT THIS IS BAD!)")
	} else {
		t.Logf("Client failed to login: %s (BUT THIS IS GOOD!)", err)
	}
}

func TestLoginNoPW(t *testing.T) {
	test := BuildUp(failedLogin, t)
	defer test.TearDown()
	err := test.client.Login("", "")
	if err != nil {
		t.Log("Client refused to login with password.")
	} else {
		t.Error("Client did not a return an error with no password set")
	}
}

func TestLoginFailed(t *testing.T) {
	test := BuildUp(failedLogin, t)
	defer test.TearDown()
	err := test.client.Login("asdf", "JKLa")
	if err != nil {
		t.Logf("Failed to log in: %s", err.Error())
	} else {
		t.Error("Client logged in successfully to incorrect response")
	}
}

func TestPostForm(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		err := r.ParseForm()
		if err != nil {
			panic(err)
		}

		if r.Header.Get("user-agent") != "mediawiki (Golang) https://github.com/sadbox/mediawiki TESTING" {
			fmt.Fprintln(w, "USERAGENT")
		} else {
			fmt.Fprintln(w, r.Form.Get("KEY"))
		}
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err.Error())
	}
	value, err := client.postForm(url.Values{"KEY": []string{"VALUE"}})
	if err != nil {
		t.Errorf("Error posting data: %s", err.Error())
	}
	returnValue := strings.TrimSpace(string(value))
	if returnValue == "VALUE" {
		t.Log("Successfully posted to web service.")
	} else if returnValue == "USERAGENT" {
		t.Error("Wrong useragent used!")
	} else {
		t.Error("Did not retrieve right value from web service")
	}
}

func TestAPI(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		err := r.ParseForm()
		if err != nil {
			panic(err)
		}
		if r.Form.Get("KEY") != "VALUE" || r.Form.Get("OTHER KEY") != "OTHER VALUE" || r.Form.Get("format") != "json" {
			fmt.Fprintln(w, `{"status":"FAIL"}`)
		} else {
			fmt.Fprintln(w, `{"status":"PASS"}`)
		}
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err.Error())
	}
	body, err := client.API(map[string]string{"KEY": "VALUE", "OTHER KEY": "OTHER VALUE"})
	if err != nil {
		t.Fatalf("API() returned a non-nil error: %s", err.Error())
	}
	if strings.TrimSpace(string(body)) == `{"status":"PASS"}` {
		t.Log("Successfully posted all information via API() call")
	} else {
		t.Error("Did not get PASS back from test server when posting via API()")
	}
}

func TestRead(t *testing.T) {
	test := BuildUp(readPage, t)
	defer test.TearDown()
	page, err := test.client.Read("TESTING PAGE")
	if err != nil {
		t.Fatalf("Unable to read page: %s", err)
	}
	if page.Revisions[0].Body != "FULL PAGE TEXT" {
		t.Error("Page content not correct")
	}
}

func TestDownload(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		err := r.ParseForm()
		if err != nil {
			panic(err)
		}
		if r.Method == "POST" {
			fmt.Fprintln(w, fmt.Sprintf(fileURL, r.Form.Get("titles")))
		} else if r.Method == "GET" {
			fmt.Fprintf(w, `THINGS`)
		}
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err.Error())
	}
	file, err := client.Download(ts.URL)
	if err != nil {
		t.Fatalf("Error downloading file: %s", err.Error())
	}
	defer file.Close()
	returned, err := ioutil.ReadAll(file)
	if err != nil {
		t.Fatalf("Error reading downloaded file: %s", err.Error())
	}
	if string(returned) != "THINGS" {
		t.Fatalf("Returned file was not correct")
	}
}

func TestDownloadNoFiles(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		err := r.ParseForm()
		if err != nil {
			panic(err)
		}
		if r.Method == "POST" {
			fmt.Fprintln(w, fileURLFailed)
		} else if r.Method == "GET" {
			fmt.Fprintf(w, `THINGS`)
		}
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err)
	}
	_, err = client.Download(ts.URL)
	if err != nil {
		t.Log("Successfully returned error when no files were found", err)
	} else {
		t.Fatal("No error return when no files were found", err)
	}
}

func TestUpload(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		err := r.ParseMultipartForm(int64(10000))
		if err != nil {
			panic(err)
		}
		formValues := r.MultipartForm.Value
		referenceValues := map[string]string{
			"action":   "upload",
			"format":   "json",
			"filename": "test.txt",
			"token":    "ASDFASDF",
		}
	NextKey:
		for key, value := range formValues {
			for innerKey, innerValue := range referenceValues {
				if key == innerKey && value[0] == innerValue {
					continue NextKey
				}
			}
			fmt.Fprintln(w, fmt.Sprintf(`{"upload":{"result":"Value did not match: %s"}}`, key))
			return
		}
		uploadedFile, err := r.MultipartForm.File["file"][0].Open()
		if err != nil {
			fmt.Fprintln(w, `{"upload":{"result":"Error opening uploaded file"}}`)
			return
		}
		defer uploadedFile.Close()
		contents, err := ioutil.ReadAll(uploadedFile)
		if err != nil {
			panic(err)
		}
		if string(contents) != "THIS IS A TEST" {
			fmt.Fprintln(w, `{"upload":{"result":"File contents are not valid"}}`)
			return
		}
		fmt.Fprintln(w, `{"upload":{"result":"Success"}}`)
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err.Error())
	}
	client.edittoken = "ASDFASDF"
	err = client.Upload("test.txt", strings.NewReader("THIS IS A TEST"))
	if err != nil {
		t.Fatalf("Error trying to upload file: %s", err)
	}
}

func TestUploadAutoToken(t *testing.T) {
	test := BuildUp(editTokenReponse, t)
	defer test.TearDown()
	test.client.Upload("stuff", strings.NewReader("stuff"))
	if test.client.edittoken == "" {
		t.Fatalf("Edit token did not get set properly")
	}
}

func TestUploadFailResponse(t *testing.T) {
	test := BuildUp(`{"upload":{"result":"THIS SHOULD BE AN ERROR"}}`, t)
	defer test.TearDown()
	test.client.edittoken = "ASDF"
	err := test.client.Upload("stuff", strings.NewReader("stuff"))
	if err == nil {
		t.Fatal("Did not generate error when upload returned failed result", err)
	} else {
		t.Log("Successfully generated error from failed upload", err)
	}
}

func TestMWError(t *testing.T) {
	test := BuildUp(mwerror, t)
	defer test.TearDown()
	_, err := test.client.Read("DOESN'T MATTER")
	if err != nil {
		t.Log("Properly recieved error:", err)
	} else {
		t.Fatalf("Mediawiki error did not get translated to a go error")
	}
}

func TestEditAutoToken(t *testing.T) {
	test := BuildUp(editTokenReponse, t)
	defer test.TearDown()
	test.client.Edit(map[string]string{"thing": "OTHER THING"})
	if test.client.edittoken == "" {
		t.Fatalf("Edit token did not get set properly")
	}
}

func TestEditSuccess(t *testing.T) {
	test := BuildUp(editsuccess, t)
	defer test.TearDown()
	test.client.edittoken = "asdf"
	err := test.client.Edit(map[string]string{"title": "somepage"})
	if err != nil {
		t.Fatal("Did not get non-error response back", err)
	}
}

func TestEditFail(t *testing.T) {
	test := BuildUp(editfailure, t)
	defer test.TearDown()
	err := test.client.Edit(map[string]string{"title": "somepage"})
	if err == nil {
		t.Fatal("Did not get non-error response back", err)
	}
}

func TestBasicAuth(t *testing.T) {
	ts := httptest.NewServer(http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
		if r.Header.Get("Authorization") != "Basic Zm9vOmJhcg==" {
			t.Fatalf("Did not recieve correct basic auth header: %s", r.Header.Get(r.Header.Get("Authorization")))
		}
	}))
	defer ts.Close()
	client, err := New(ts.URL, "TESTING")
	if err != nil {
		t.Fatalf("Error creating client: %s", err.Error())
	}

	client.UseBasicAuth = true
	client.BasicAuthUser = "foo"
	client.BasicAuthPass = "bar"

	t.Log(client)

	_, err = client.API()
	if err != nil {
		t.Fatalf("API() returned a non-nil error: %s", err.Error())
	}
}0x5191e669813cd52ce03fca7487c6208FCodeAlphabet(uint32_t bits, uint16_t* alphabet, size_t* nbits)
title: Audio Output Devices API
slug: Web/API/Audio_Output_Devices_API
page-type: web-api-overview
status:
  - experimental
browser-compat:
  - api.MediaDevices.selectAudioOutput
  - api.HTMLMediaElement.setSinkId
  - api.HTMLMediaElement.sinkId
  - http.headers.Permissions-Policy.speaker-selection
spec-urls: https://w3c.github.io/mediacapture-output/#dom-mediadevices-selectaudiooutput
---

{{DefaultAPISidebar("Audio Output Devices API")}}{{securecontext_header}}{{SeeCompatTable}}

The **Audio Output Devices API** allows web applications to prompt users about what output device should be used for audio playback.

## Concepts and usage

Operating systems commonly allow users to specify that audio should be played from speakers, a Bluetooth headset, or some other audio output device.
This API allows applications to provide this same functionality from within a web page.

Even if allowed by a permission policy, access to a particular audio output device still requires explicit user permission, as the user may be in a location where playing audio through some output devices is not appropriate.

The API provides the [`MediaDevices.selectAudioOutput()`](/en-US/docs/Web/API/MediaDevices/selectAudioOutput) method that allows users to select their desired audio output from those that are allowed by the [`speaker-selection`](/en-US/docs/Web/HTTP/Headers/Permissions-Policy/speaker-selection) directive of the [`Permissions-Policy`](/en-US/docs/Web/HTTP/Headers/Permissions-Policy) HTTP header for the document.
The selected device then has user permission, allowing it to be enumerated with [`MediaDevices.enumerateDevices()`](/en-US/docs/Web/API/MediaDevices/enumerateDevices) and set as the audio output device using [`HTMLMediaElement.setSinkId()`](/en-US/docs/Web/API/HTMLMediaElement/setSinkId).

Audio devices may arbitrarily connect and disconnect.
Applications that wish to react to this kind of change can listen to the [`devicechange` event](/en-US/docs/Web/API/MediaDevices/devicechange_event) and use [`enumerateDevices()`](/en-US/docs/Web/API/MediaDevices/enumerateDevices) to determine if `sinkId` is present in the returned devices.
This might trigger, for example, pausing or unpausing playback.

## Interfaces

### Extensions to interfaces

The Audio Output Devices API extends the following APIs, adding the listed features:

#### MediaDevices

- [`MediaDevices.selectAudioOutput()`](/en-US/docs/Web/API/MediaDevices/selectAudioOutput)
  - : This method prompts the user to select a specific audio output device, for example a speaker or headset.
    Selecting a device grants user permission to use that device and returns information about the device, including its ID.

#### HTMLMediaElement

- [`HTMLMediaElement.setSinkId()`](/en-US/docs/Web/API/HTMLMediaElement/setSinkId)
  - : This method sets the ID of the audio device to use for output, which will be used if permitted.
- [`HTMLMediaElement.sinkId`](/en-US/docs/Web/API/HTMLMediaElement/sinkId)
  - : This property returns the unique ID of the audio device being used for output, or an empty string if the default user agent device is being used.

## Security requirements

Access to the API is subject to the following constraints:

- All methods and properties may only be called in a [secure context](/en-US/docs/Web/Security/Secure_Contexts).

- [`MediaDevices.selectAudioOutput()`](/en-US/docs/Web/API/MediaDevices/selectAudioOutput) grants user permission for a selected device to be used as the audio output sink:

  - Access may be gated by the [`speaker-selection`](/en-US/docs/Web/HTTP/Headers/Permissions-Policy/speaker-selection) HTTP [Permission Policy](/en-US/docs/Web/HTTP/Permissions_Policy).
  - [Transient user activation](/en-US/docs/Web/Security/User_activation) is required.
    The user has to interact with the page or a UI element for the method to be called.

- [`HTMLMediaElement.setSinkId()`](/en-US/docs/Web/API/HTMLMediaElement/setSinkId) sets a permitted ID as the audio output:

  - Access may be gated by the [`speaker-selection`](/en-US/docs/Web/HTTP/Headers/Permissions-Policy/speaker-selection) HTTP [Permission Policy](/en-US/docs/Web/HTTP/Permissions_Policy).
  - User permission is required to set a non-default device ID.
    - This can come from selection in the prompt launched by `MediaDevices.selectAudioOutput()`
    - User permission to set the output device is also implicitly granted if the user has already granted permission to use a media input device in the same group with [`MediaDevices.getUserMedia()`](/en-US/docs/Web/API/MediaDevices/getUserMedia).

The permission status can be queried using the [Permissions API](/en-US/docs/Web/API/Permissions_API) method [`navigator.permissions.query()`](/en-US/docs/Web/API/Permissions/query), passing a permission descriptor with the `speaker-selection` permission.

## Examples

Here's an example of using `selectAudioOutput()`, within a function that is triggered by a button click, and then setting the selected device as the audio output.

The code first checks if `selectAudioOutput()` is supported, and if it is, uses it to select an output and return a [device ID](/en-US/docs/Web/API/MediaDeviceInfo/deviceId).
We then play some audio using the default output, and then call `setSinkId()` in order to switch to the selected output device.

```js
document.querySelector("#myButton").addEventListener("click", async () => {
  if (!navigator.mediaDevices.selectAudioOutput) {
    console.log("selectAudioOutput() not supported or not in secure context.");
    return;
  }

  // Display prompt to select device
  const audioDevice = await navigator.mediaDevices.selectAudioOutput();

  // Create an audio element and start playing audio on the default device
  const audio = document.createElement("audio");
  audio.src = "https://example.com/audio.mp3";
  audio.play();

  // Change the sink to the selected audio output device.
  audio.setSinkId(audioDevice.deviceId);
});
```

Note that if you log the output details, they might look something like this:

```js
console.log(
  `${audioDevice.kind}: ${audioDevice.label} id = ${audioDevice.deviceId}`,
);
// audiooutput: Realtek Digital Output (Realtek(R) Audio) id = 0wE6fURSZ20H0N2NbxqgowQJLWbwo+5ablCVVJwRM3k=
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
