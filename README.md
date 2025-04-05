version: 1
frontend:
  phases:
    preBuild:
      commands:
        - corepack enable
        - npm install
    build:
      commands:
        - npm run build
  artifacts:
    baseDirectory: .amplify-hosting
    files:
      - '**/*'
