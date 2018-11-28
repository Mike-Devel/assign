cmake_minimum_required(VERSION 3.5)
project(BoostAssign)

add_library(boost_assign INTERFACE)
add_library(Boost::assign ALIAS boost_assign)

target_include_directories(boost_assign INTERFACE include)

target_link_libraries(boost_assign
	INTERFACE
		Boost::array
		Boost::config
		Boost::core
		Boost::move
		Boost::mpl
		Boost::preprocessor
		Boost::ptr_container
		Boost::range
		Boost::static_assert
		Boost::throw_exception
		Boost::tuple
		Boost::type_traits
)

