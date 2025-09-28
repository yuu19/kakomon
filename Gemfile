source "https://rubygems.org"

gem "github-pages", group: :jekyll_plugins
# github-pages は webrick を依存に含まないのでローカル開発で必要
install_if -> { RUBY_VERSION < "3.0" } do
gem "webrick"
end
