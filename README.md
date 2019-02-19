# kirangautam
Personal Website

Userful Alias:
alias uploadS3='aws s3 sync . s3://kirangautam.com'
DID=E11MP5G9W22WDN
invalidateCF ()
{
echo "Running: aws cloudfront create-invalidation --distribution-id $@ --paths \"/*\""
aws cloudfront create-invalidation --distribution-id $@ --paths "/*"
}
- uploadS3
- invalidateCF $DID