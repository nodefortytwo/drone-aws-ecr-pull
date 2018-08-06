# drone-aws-ecr-pull
Pulls image from private ECR

## Drone configuration examples

```yaml
pipeline:
  pull:
    image: nodefortytwo/drone-aws-ecr-pull
    images:
        - 99999.dkr.ecr.us-east-1.amazonaws.com/build_image
    privileged: true
    volumes:
      - /var/run/docker.sock:/var/run/docker.sock
```
