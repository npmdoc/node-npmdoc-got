# api documentation for  [got (v6.7.1)](https://github.com/sindresorhus/got#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-got.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-got) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-got.svg)](https://travis-ci.org/npmdoc/node-npmdoc-got)
#### Simplified HTTP requests

[![NPM](https://nodei.co/npm/got.png?downloads=true)](https://www.npmjs.com/package/got)

[![apidoc](https://npmdoc.github.io/node-npmdoc-got/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-got%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-got/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-got/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-got/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "ava": {
        "concurrency": 4
    },
    "browser": {
        "unzip-response": false
    },
    "bugs": {
        "url": "https://github.com/sindresorhus/got/issues"
    },
    "dependencies": {
        "create-error-class": "^3.0.0",
        "duplexer3": "^0.1.4",
        "get-stream": "^3.0.0",
        "is-redirect": "^1.0.0",
        "is-retry-allowed": "^1.0.0",
        "is-stream": "^1.0.0",
        "lowercase-keys": "^1.0.0",
        "safe-buffer": "^5.0.1",
        "timed-out": "^4.0.0",
        "unzip-response": "^2.0.1",
        "url-parse-lax": "^1.0.0"
    },
    "description": "Simplified HTTP requests",
    "devDependencies": {
        "ava": "^0.17.0",
        "coveralls": "^2.11.4",
        "form-data": "^2.1.1",
        "get-port": "^2.0.0",
        "into-stream": "^3.0.0",
        "nyc": "^10.0.0",
        "pem": "^1.4.4",
        "pify": "^2.3.0",
        "tempfile": "^1.1.1",
        "xo": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "240cd05785a9a18e561dc1b44b41c763ef1e8db0",
        "tarball": "https://registry.npmjs.org/got/-/got-6.7.1.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "52da6067ddac5250d6c2e76af9a150b9cf4ba025",
    "homepage": "https://github.com/sindresorhus/got#readme",
    "keywords": [
        "http",
        "https",
        "get",
        "got",
        "url",
        "uri",
        "request",
        "util",
        "utility",
        "simple",
        "curl",
        "wget",
        "fetch"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "sindresorhus",
            "email": "sindresorhus@gmail.com"
        },
        {
            "name": "floatdrop",
            "email": "floatdrop@gmail.com"
        },
        {
            "name": "kevva",
            "email": "kevinmartensson@gmail.com"
        }
    ],
    "name": "got",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sindresorhus/got.git"
    },
    "scripts": {
        "coveralls": "nyc report --reporter=text-lcov | coveralls",
        "test": "xo && nyc ava"
    },
    "version": "6.7.1",
    "xo": {
        "esnext": true
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module got](#apidoc.module.got)
1.  [function <span class="apidocSignatureSpan">got.</span>HTTPError ()](#apidoc.element.got.HTTPError)
1.  [function <span class="apidocSignatureSpan">got.</span>HTTPError.super_ ()](#apidoc.element.got.HTTPError.super_)
1.  [function <span class="apidocSignatureSpan">got.</span>MaxRedirectsError ()](#apidoc.element.got.MaxRedirectsError)
1.  [function <span class="apidocSignatureSpan">got.</span>ParseError ()](#apidoc.element.got.ParseError)
1.  [function <span class="apidocSignatureSpan">got.</span>ReadError ()](#apidoc.element.got.ReadError)
1.  [function <span class="apidocSignatureSpan">got.</span>RequestError ()](#apidoc.element.got.RequestError)
1.  [function <span class="apidocSignatureSpan">got.</span>delete (url, opts)](#apidoc.element.got.delete)
1.  [function <span class="apidocSignatureSpan">got.</span>get (url, opts)](#apidoc.element.got.get)
1.  [function <span class="apidocSignatureSpan">got.</span>head (url, opts)](#apidoc.element.got.head)
1.  [function <span class="apidocSignatureSpan">got.</span>patch (url, opts)](#apidoc.element.got.patch)
1.  [function <span class="apidocSignatureSpan">got.</span>post (url, opts)](#apidoc.element.got.post)
1.  [function <span class="apidocSignatureSpan">got.</span>put (url, opts)](#apidoc.element.got.put)
1.  [function <span class="apidocSignatureSpan">got.</span>stream (url, opts)](#apidoc.element.got.stream)

#### [module got.HTTPError](#apidoc.module.got.HTTPError)
1.  [function <span class="apidocSignatureSpan">got.</span>HTTPError ()](#apidoc.element.got.HTTPError.HTTPError)
1.  [function <span class="apidocSignatureSpan">got.HTTPError.</span>super_ ()](#apidoc.element.got.HTTPError.super_)

#### [module got.HTTPError.super_](#apidoc.module.got.HTTPError.super_)
1.  [function <span class="apidocSignatureSpan">got.HTTPError.</span>super_ ()](#apidoc.element.got.HTTPError.super_.super_)
1.  [function <span class="apidocSignatureSpan">got.HTTPError.super_.</span>captureStackTrace ()](#apidoc.element.got.HTTPError.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">got.HTTPError.super_.</span>stackTraceLimit

#### [module got.MaxRedirectsError](#apidoc.module.got.MaxRedirectsError)
1.  [function <span class="apidocSignatureSpan">got.</span>MaxRedirectsError ()](#apidoc.element.got.MaxRedirectsError.MaxRedirectsError)
1.  [function <span class="apidocSignatureSpan">got.MaxRedirectsError.</span>super_ ()](#apidoc.element.got.MaxRedirectsError.super_)

#### [module got.ParseError](#apidoc.module.got.ParseError)
1.  [function <span class="apidocSignatureSpan">got.</span>ParseError ()](#apidoc.element.got.ParseError.ParseError)
1.  [function <span class="apidocSignatureSpan">got.ParseError.</span>super_ ()](#apidoc.element.got.ParseError.super_)

#### [module got.ReadError](#apidoc.module.got.ReadError)
1.  [function <span class="apidocSignatureSpan">got.</span>ReadError ()](#apidoc.element.got.ReadError.ReadError)
1.  [function <span class="apidocSignatureSpan">got.ReadError.</span>super_ ()](#apidoc.element.got.ReadError.super_)

#### [module got.RequestError](#apidoc.module.got.RequestError)
1.  [function <span class="apidocSignatureSpan">got.</span>RequestError ()](#apidoc.element.got.RequestError.RequestError)
1.  [function <span class="apidocSignatureSpan">got.RequestError.</span>super_ ()](#apidoc.element.got.RequestError.super_)

#### [module got.stream](#apidoc.module.got.stream)
1.  [function <span class="apidocSignatureSpan">got.</span>stream (url, opts)](#apidoc.element.got.stream.stream)
1.  [function <span class="apidocSignatureSpan">got.stream.</span>delete (url, opts)](#apidoc.element.got.stream.delete)
1.  [function <span class="apidocSignatureSpan">got.stream.</span>get (url, opts)](#apidoc.element.got.stream.get)
1.  [function <span class="apidocSignatureSpan">got.stream.</span>head (url, opts)](#apidoc.element.got.stream.head)
1.  [function <span class="apidocSignatureSpan">got.stream.</span>patch (url, opts)](#apidoc.element.got.stream.patch)
1.  [function <span class="apidocSignatureSpan">got.stream.</span>post (url, opts)](#apidoc.element.got.stream.post)
1.  [function <span class="apidocSignatureSpan">got.stream.</span>put (url, opts)](#apidoc.element.got.stream.put)



# <a name="apidoc.module.got"></a>[module got](#apidoc.module.got)

#### <a name="apidoc.element.got.HTTPError"></a>[function <span class="apidocSignatureSpan">got.</span>HTTPError ()](#apidoc.element.got.HTTPError)
- description and source-code
```javascript
HTTPError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
							res.body = JSON.parse(res.body);
						} catch (e) {
							throw new got.ParseError(e, statusCode, opts, data);
						}
					}

					if (statusCode < 200 || statusCode > limitStatusCode) {
						throw new got.HTTPError(statusCode, opts);
					}

					resolve(res);
				})
				.catch(err => {
					Object.defineProperty(err, 'response', {value: res});
					reject(err);
...
```

#### <a name="apidoc.element.got.HTTPError.super_"></a>[function <span class="apidocSignatureSpan">got.</span>HTTPError.super_ ()](#apidoc.element.got.HTTPError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.got.MaxRedirectsError"></a>[function <span class="apidocSignatureSpan">got.</span>MaxRedirectsError ()](#apidoc.element.got.MaxRedirectsError)
- description and source-code
```javascript
MaxRedirectsError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
		const req = fn.request(opts, res => {
			const statusCode = res.statusCode;

			if (isRedirect(statusCode) && opts.followRedirect && 'location' in res.headers && (opts.method === 'GET' || opts.method === '
HEAD')) {
				res.resume();

				if (++redirectCount > 10) {
					ee.emit('error', new got.MaxRedirectsError(statusCode, opts), null, res);
					return;
				}

				const bufferString = Buffer.from(res.headers.location, 'binary').toString();

				redirectUrl = urlLib.resolve(urlLib.format(opts), bufferString);
				const redirectOpts = Object.assign({}, opts, urlLib.parse(redirectUrl));
...
```

#### <a name="apidoc.element.got.ParseError"></a>[function <span class="apidocSignatureSpan">got.</span>ParseError ()](#apidoc.element.got.ParseError)
- description and source-code
```javascript
ParseError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...

					res.body = data;

					if (opts.json && res.body) {
						try {
							res.body = JSON.parse(res.body);
						} catch (e) {
							throw new got.ParseError(e, statusCode, opts, data);
						}
					}

					if (statusCode < 200 || statusCode > limitStatusCode) {
						throw new got.HTTPError(statusCode, opts);
					}
...
```

#### <a name="apidoc.element.got.ReadError"></a>[function <span class="apidocSignatureSpan">got.</span>ReadError ()](#apidoc.element.got.ReadError)
- description and source-code
```javascript
ReadError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
			req.end(opts.body);
		});

		ee.on('response', res => {
			const stream = opts.encoding === null ? getStream.buffer(res) : getStream(res, opts);

			stream
				.catch(err => reject(new got.ReadError(err, opts)))
				.then(data => {
					const statusCode = res.statusCode;
					const limitStatusCode = opts.followRedirect ? 299 : 399;

					res.body = data;

					if (opts.json && res.body) {
...
```

#### <a name="apidoc.element.got.RequestError"></a>[function <span class="apidocSignatureSpan">got.</span>RequestError ()](#apidoc.element.got.RequestError)
- description and source-code
```javascript
RequestError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
			const backoff = opts.retries(++retryCount, err);

			if (backoff) {
				setTimeout(get, backoff, opts);
				return;
			}

			ee.emit('error', new got.RequestError(err, opts));
		});

		if (opts.gotTimeout) {
			timedOut(req, opts.gotTimeout);
		}

		setImmediate(() => {
...
```

#### <a name="apidoc.element.got.delete"></a>[function <span class="apidocSignatureSpan">got.</span>delete (url, opts)](#apidoc.element.got.delete)
- description and source-code
```javascript
(url, opts) => got(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...
'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.


## Errors

Each error contains (if available) 'statusCode', 'statusMessage', 'host', 'hostname', 'method' and 'path' properties to make debugging
 easier.
...
```

#### <a name="apidoc.element.got.get"></a>[function <span class="apidocSignatureSpan">got.</span>get (url, opts)](#apidoc.element.got.get)
- description and source-code
```javascript
(url, opts) => got(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...

'redirect' event to get the response object of a redirect. The second argument is options for the next request to the redirect location
.

##### .on('error', error, body, response)

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.
...
```

#### <a name="apidoc.element.got.head"></a>[function <span class="apidocSignatureSpan">got.</span>head (url, opts)](#apidoc.element.got.head)
- description and source-code
```javascript
(url, opts) => got(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.


## Errors
...
```

#### <a name="apidoc.element.got.patch"></a>[function <span class="apidocSignatureSpan">got.</span>patch (url, opts)](#apidoc.element.got.patch)
- description and source-code
```javascript
(url, opts) => got(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...
##### .on('error', error, body, response)

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.


## Errors
...
```

#### <a name="apidoc.element.got.post"></a>[function <span class="apidocSignatureSpan">got.</span>post (url, opts)](#apidoc.element.got.post)
- description and source-code
```javascript
(url, opts) => got(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...
		//=> 'Internal server error ...'
	});

// Streams
got.stream('todomvc.com').pipe(fs.createWriteStream('index.html'));

// For POST, PUT and PATCH methods got.stream returns a WritableStream
fs.createReadStream('index.html').pipe(got.stream.post('todomvc.com'));
'''


### API

It's a 'GET' request by default, but can be changed in 'options'.
...
```

#### <a name="apidoc.element.got.put"></a>[function <span class="apidocSignatureSpan">got.</span>put (url, opts)](#apidoc.element.got.put)
- description and source-code
```javascript
(url, opts) => got(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...

##### .on('error', error, body, response)

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.
...
```

#### <a name="apidoc.element.got.stream"></a>[function <span class="apidocSignatureSpan">got.</span>stream (url, opts)](#apidoc.element.got.stream)
- description and source-code
```javascript
(url, opts) => asStream(normalizeArguments(url, opts))
```
- example usage
```shell
...
helpers.forEach(el => {
	got[el] = (url, opts) => got(url, Object.assign({}, opts, {method: el}));
});

got.stream = (url, opts) => asStream(normalizeArguments(url, opts));

for (const el of helpers) {
	got.stream[el] = (url, opts) => got.stream(url, Object.assign({}, opts, {method: el}));
}

function stdError(error, opts) {
	if (error.code !== undefined) {
		this.code = error.code;
	}
...
```



# <a name="apidoc.module.got.HTTPError"></a>[module got.HTTPError](#apidoc.module.got.HTTPError)

#### <a name="apidoc.element.got.HTTPError.HTTPError"></a>[function <span class="apidocSignatureSpan">got.</span>HTTPError ()](#apidoc.element.got.HTTPError.HTTPError)
- description and source-code
```javascript
HTTPError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
							res.body = JSON.parse(res.body);
						} catch (e) {
							throw new got.ParseError(e, statusCode, opts, data);
						}
					}

					if (statusCode < 200 || statusCode > limitStatusCode) {
						throw new got.HTTPError(statusCode, opts);
					}

					resolve(res);
				})
				.catch(err => {
					Object.defineProperty(err, 'response', {value: res});
					reject(err);
...
```

#### <a name="apidoc.element.got.HTTPError.super_"></a>[function <span class="apidocSignatureSpan">got.HTTPError.</span>super_ ()](#apidoc.element.got.HTTPError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.got.HTTPError.super_"></a>[module got.HTTPError.super_](#apidoc.module.got.HTTPError.super_)

#### <a name="apidoc.element.got.HTTPError.super_.super_"></a>[function <span class="apidocSignatureSpan">got.HTTPError.</span>super_ ()](#apidoc.element.got.HTTPError.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.got.HTTPError.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">got.HTTPError.super_.</span>captureStackTrace ()](#apidoc.element.got.HTTPError.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.got.MaxRedirectsError"></a>[module got.MaxRedirectsError](#apidoc.module.got.MaxRedirectsError)

#### <a name="apidoc.element.got.MaxRedirectsError.MaxRedirectsError"></a>[function <span class="apidocSignatureSpan">got.</span>MaxRedirectsError ()](#apidoc.element.got.MaxRedirectsError.MaxRedirectsError)
- description and source-code
```javascript
MaxRedirectsError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
		const req = fn.request(opts, res => {
			const statusCode = res.statusCode;

			if (isRedirect(statusCode) && opts.followRedirect && 'location' in res.headers && (opts.method === 'GET' || opts.method === '
HEAD')) {
				res.resume();

				if (++redirectCount > 10) {
					ee.emit('error', new got.MaxRedirectsError(statusCode, opts), null, res);
					return;
				}

				const bufferString = Buffer.from(res.headers.location, 'binary').toString();

				redirectUrl = urlLib.resolve(urlLib.format(opts), bufferString);
				const redirectOpts = Object.assign({}, opts, urlLib.parse(redirectUrl));
...
```

#### <a name="apidoc.element.got.MaxRedirectsError.super_"></a>[function <span class="apidocSignatureSpan">got.MaxRedirectsError.</span>super_ ()](#apidoc.element.got.MaxRedirectsError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.got.ParseError"></a>[module got.ParseError](#apidoc.module.got.ParseError)

#### <a name="apidoc.element.got.ParseError.ParseError"></a>[function <span class="apidocSignatureSpan">got.</span>ParseError ()](#apidoc.element.got.ParseError.ParseError)
- description and source-code
```javascript
ParseError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...

					res.body = data;

					if (opts.json && res.body) {
						try {
							res.body = JSON.parse(res.body);
						} catch (e) {
							throw new got.ParseError(e, statusCode, opts, data);
						}
					}

					if (statusCode < 200 || statusCode > limitStatusCode) {
						throw new got.HTTPError(statusCode, opts);
					}
...
```

#### <a name="apidoc.element.got.ParseError.super_"></a>[function <span class="apidocSignatureSpan">got.ParseError.</span>super_ ()](#apidoc.element.got.ParseError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.got.ReadError"></a>[module got.ReadError](#apidoc.module.got.ReadError)

#### <a name="apidoc.element.got.ReadError.ReadError"></a>[function <span class="apidocSignatureSpan">got.</span>ReadError ()](#apidoc.element.got.ReadError.ReadError)
- description and source-code
```javascript
ReadError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
			req.end(opts.body);
		});

		ee.on('response', res => {
			const stream = opts.encoding === null ? getStream.buffer(res) : getStream(res, opts);

			stream
				.catch(err => reject(new got.ReadError(err, opts)))
				.then(data => {
					const statusCode = res.statusCode;
					const limitStatusCode = opts.followRedirect ? 299 : 399;

					res.body = data;

					if (opts.json && res.body) {
...
```

#### <a name="apidoc.element.got.ReadError.super_"></a>[function <span class="apidocSignatureSpan">got.ReadError.</span>super_ ()](#apidoc.element.got.ReadError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.got.RequestError"></a>[module got.RequestError](#apidoc.module.got.RequestError)

#### <a name="apidoc.element.got.RequestError.RequestError"></a>[function <span class="apidocSignatureSpan">got.</span>RequestError ()](#apidoc.element.got.RequestError.RequestError)
- description and source-code
```javascript
RequestError = function () {
		Object.defineProperty(this, 'name', {
			configurable: true,
			value: className,
			writable: true
		});

		captureStackTrace(this, this.constructor);

		setup.apply(this, arguments);
	}
```
- example usage
```shell
...
			const backoff = opts.retries(++retryCount, err);

			if (backoff) {
				setTimeout(get, backoff, opts);
				return;
			}

			ee.emit('error', new got.RequestError(err, opts));
		});

		if (opts.gotTimeout) {
			timedOut(req, opts.gotTimeout);
		}

		setImmediate(() => {
...
```

#### <a name="apidoc.element.got.RequestError.super_"></a>[function <span class="apidocSignatureSpan">got.RequestError.</span>super_ ()](#apidoc.element.got.RequestError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.got.stream"></a>[module got.stream](#apidoc.module.got.stream)

#### <a name="apidoc.element.got.stream.stream"></a>[function <span class="apidocSignatureSpan">got.</span>stream (url, opts)](#apidoc.element.got.stream.stream)
- description and source-code
```javascript
(url, opts) => asStream(normalizeArguments(url, opts))
```
- example usage
```shell
...
helpers.forEach(el => {
	got[el] = (url, opts) => got(url, Object.assign({}, opts, {method: el}));
});

got.stream = (url, opts) => asStream(normalizeArguments(url, opts));

for (const el of helpers) {
	got.stream[el] = (url, opts) => got.stream(url, Object.assign({}, opts, {method: el}));
}

function stdError(error, opts) {
	if (error.code !== undefined) {
		this.code = error.code;
	}
...
```

#### <a name="apidoc.element.got.stream.delete"></a>[function <span class="apidocSignatureSpan">got.stream.</span>delete (url, opts)](#apidoc.element.got.stream.delete)
- description and source-code
```javascript
(url, opts) => got.stream(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...
'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.


## Errors

Each error contains (if available) 'statusCode', 'statusMessage', 'host', 'hostname', 'method' and 'path' properties to make debugging
 easier.
...
```

#### <a name="apidoc.element.got.stream.get"></a>[function <span class="apidocSignatureSpan">got.stream.</span>get (url, opts)](#apidoc.element.got.stream.get)
- description and source-code
```javascript
(url, opts) => got.stream(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...

'redirect' event to get the response object of a redirect. The second argument is options for the next request to the redirect location
.

##### .on('error', error, body, response)

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.
...
```

#### <a name="apidoc.element.got.stream.head"></a>[function <span class="apidocSignatureSpan">got.stream.</span>head (url, opts)](#apidoc.element.got.stream.head)
- description and source-code
```javascript
(url, opts) => got.stream(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.


## Errors
...
```

#### <a name="apidoc.element.got.stream.patch"></a>[function <span class="apidocSignatureSpan">got.stream.</span>patch (url, opts)](#apidoc.element.got.stream.patch)
- description and source-code
```javascript
(url, opts) => got.stream(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...
##### .on('error', error, body, response)

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.


## Errors
...
```

#### <a name="apidoc.element.got.stream.post"></a>[function <span class="apidocSignatureSpan">got.stream.</span>post (url, opts)](#apidoc.element.got.stream.post)
- description and source-code
```javascript
(url, opts) => got.stream(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...
		//=> 'Internal server error ...'
	});

// Streams
got.stream('todomvc.com').pipe(fs.createWriteStream('index.html'));

// For POST, PUT and PATCH methods got.stream returns a WritableStream
fs.createReadStream('index.html').pipe(got.stream.post('todomvc.com'));
'''


### API

It's a 'GET' request by default, but can be changed in 'options'.
...
```

#### <a name="apidoc.element.got.stream.put"></a>[function <span class="apidocSignatureSpan">got.stream.</span>put (url, opts)](#apidoc.element.got.stream.put)
- description and source-code
```javascript
(url, opts) => got.stream(url, Object.assign({}, opts, {method: el}))
```
- example usage
```shell
...

##### .on('error', error, body, response)

'error' event emitted in case of protocol error (like 'ENOTFOUND' etc.) or status error (4xx or 5xx). The second argument is the
 body of the server response in case of status error. The third argument is response object.

#### got.get(url, [options])
#### got.post(url, [options])
#### got.put(url, [options])
#### got.patch(url, [options])
#### got.head(url, [options])
#### got.delete(url, [options])

Sets 'options.method' to the method name and makes a request.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
