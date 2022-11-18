# CI/CD for ETHX

Continuous Integration and Continuous Delivery for ETHX

## Staging environment for all PRs

`deploy-staging-aws`

1. Checkout smart contracts repo
2. Checkout frontend (dapp) repo
3. Compile smart contracts
4. Compile and build frontend repo
5. Deploy smart contracts to Tenderly fork using JSON deployment params
6. Bundle smart contracts with frontend
7. Deploy the bundle to AWS S3
8. Delete everything once PR is deleted

## Prod environment for main branch

`deploy-prod`

1. Checkout smart contracts repo
2. Checkout frontend (dapp) repo
3. Compile smart contracts
4. Compile and build frontend repo
5. Deploy smart contracts to mainnet using JSON deployment params
6. Bundle smart contracts with frontend
7. Deploy the bundle to AWS S3
