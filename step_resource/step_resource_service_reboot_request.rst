.. This is an included how-to. 

.. To reboot a node at the end of the |chef client| run:

.. code-block:: ruby

   reboot 'app_requires_reboot' do
     action :request_reboot
     reason 'Need to reboot when the run completes successfully.'
     delay_mins 5
   end
