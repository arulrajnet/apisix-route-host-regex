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

## Author

<p align="center">
  <a href="https://x.com/arulrajnet">
    <img src="https://github.com/arulrajnet.png?size=100" alt="Arulraj V" width="100" height="100" style="border-radius: 50%;" class="avatar-user">
  </a>
  <br>
  <strong>Arul</strong>
  <br>
  <a href="https://x.com/arulrajnet">
    <img src="https://img.shields.io/badge/Follow-%40arulrajnet-1DA1F2?style=for-the-badge&logo=x&logoColor=white" alt="Follow @arulrajnet on X">
  </a>
  <a href="https://github.com/arulrajnet">
    <img src="https://img.shields.io/badge/GitHub-arulrajnet-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub @arulrajnet">
  </a>
  <a href="https://linkedin.com/in/arulrajnet">
    <img src="https://custom-icon-badges.demolab.com/badge/LinkedIn-arulrajnet-0A66C2?style=for-the-badge&logo=linkedin-white&logoColor=white" alt="LinkedIn @arulrajnet">
  </a>
</p>
