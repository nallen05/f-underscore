_f-underscore_ is a tiny library of functional programming utilities placed into the
public domain

the idea is to make functional programs shorter and easier to read without resorting
to syntax [like arc's square bracket unary function syntax]

    (f (x) ..) -> (lambda (x) ..)

    (f0 ..)    -> (lambda () ..)

    (f_ ..)    -> (lambda (_) ..)

    (f_n ..)   -> (lambda (&rest _) ..)

    (f_% ..)   ~= (lambda (&rest #:%) (declare (ignore #:%)) ..)

    (setf (macro-function 'foo) (m args ..)) ~= (defmacro foo args ..)
