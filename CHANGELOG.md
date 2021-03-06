# Changelog

Items starting with DEPRECATE are important deprecation notices. For more information on the list of deprecated APIs please have a look at https://docs.docker.com/misc/deprecated/ where target removal dates can also be found.

## 0.1.3 (2016-01-07)

- Fix issue sending all network configurations for a per network request.


## 0.1.2 (2016-01-07)

### Client

- Add interface to represent the API client.
- Restrict the fields send to the update endpoint to only those that are used.
- Send network settings as part of the container create request. (docker 1.10)
- Send network settings as part of the network connect request. (docker 1.10)

### Types

- Add PidsLimit as part of the host configuration.
- Add PidsStats to show PID stats.
- Add graph storage options to host configuration.
- Add NetworkConfig and EndpointIPAMConfig structs. (docker 1.10)


## 0.1.1 (2016-01-06)

### Client

- Delegate shmSize units conversion to the consumer.

### Types

- Add warnings to the volume list reponse.
- Fix image build options:
	* use 0 as default value for shmSize.


## 0.1.0 (2016-01-04)

### Client

- Initial API client implementation.

### Types

- Initial API types implementation.
