fswatch -o . | xargs -n1 -I "{}" aws s3 cp . s3://remake-web-assets --recursive --exclude ".git/*" --profile remake