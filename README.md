# yt-dlp_cmd
List of yt-dlp commands for download

Download MP4 file with audio
```sh
yt-dlp -f 22 "url"
```

# clone all repositories for user specifed
for repo in `curl -s https://api.github.com/users/terrapower/repos?per_page=1000 |grep clone_url |awk '{print $2}'| sed 's/"\(.*\)",/\1/'`;do
git clone $repo;
done;