This modification of boost allows compilation in LLVM (which does not support fastcall with variadic templates)

Compile with the following flags: "-DBOOST_DISABLE_ASSERTS -DBOOST_NO_IOSTREAM -DBOOST_DISABLE_THREADS -D_MSC_EXTENSIONS"

This will happily compile with the following includes:
#include <boost/shared_ptr.hpp>
#include <boost/current_function.hpp>
#include <boost/shared_array.hpp>
#include <boost/scoped_array.hpp>
#include <boost/circular_buffer.hpp>
#include <boost/utility/enable_if.hpp>
#include <boost/type_traits/is_enum.hpp>
#include <boost/variant.hpp>
