It is a code of http://guides.rubyonrails.org/getting_started.html example, in this guide there is a fail of post.rb, when you add tag you must put 
class Post < ActiveRecord::Base
 attr_accessible :title, :content, :tags_attributes
end

the diferences is because is necesary add :tags_attributes, If you don't add the error is :Can't mass-assign protected attributes: tags_attributes?
