# Hướng dẫn cài đặt

***Lưu ý: Đây là hướng dẫn khi chạy local trên máy tính của bạn***

**Cài đặt ruby:**

```
sudo apt update && sudo apt install ruby-full build-essential zlib1g-dev
```

**Thiết lập môi trường để cài gem mà không cần sudo:**

```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

**Cài jekyll và bundler**

```
gem install jekyll bundler
```

**Build**

```
 sudo bundle exec jekyll build
```

Mặc định lệnh này sẽ tạo thư mục _site chứa toàn bộ site tĩnh.

**Chạy local server**

```
 sudo bundle exec jekyll serve
```