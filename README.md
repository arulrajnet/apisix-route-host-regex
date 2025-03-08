APISix Route Based on Regex in Host
===============================
This is a simple example of how to create a route in APISix based on a regex in the host.

## Requirements

- Docker
- Docker Compose

## Setup

* Clone this repository
* Run the following command in the root directory of the project:
```bash
docker-compose up -d
```

## Testing

Test using curl with the host header

```bash
curl -v -H "Host: pihole-device.local.arulraj.net" http://localhost:9080 | grep -i "I am a Device!"
curl -v -H "Host: customer.local.arulraj.net" http://localhost:9080 | grep -i "This is Customer Home."
curl -v -H "Host: local.arulraj.net" http://localhost:9080 | grep -i "This is Customer Home."
```

## Cleanup

To stop the containers, run the following command:
```bash
docker-compose down
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

**Author**

| [![follow][avatar]][xhandle] |
|---|
| [@arulrajnet][xhandle] |


[xhandle]: https://x.com/arulrajnet "Follow @arulrajnet on X"
[avatar]: https://avatars0.githubusercontent.com/u/834529?s=70
