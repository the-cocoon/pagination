# Pagination

Just Pagination conerns

> params => per_page | page

@posts = Post.pagination(params)

span.mr40
  span.mr10 элементов на стр:
  - %w[ 5 10 20 50 100 125 ].each do |num|
    span.mr10= link_to num, url_for(per_page: num)

