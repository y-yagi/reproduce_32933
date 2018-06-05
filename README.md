```
unless User.exists?
  User.create!
end

p User.first.avatar.attach(io: File.open(Rails.root.join("public", "favicon.ico")), filename: 'favicon.ico')
p User.first.avatar
```
